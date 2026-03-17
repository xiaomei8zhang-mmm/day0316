# 接口测试点总结

## 1. 测试范围概览

- 数据来源：`test_cases/all_api_test_cases.csv`
- 接口总数：7
- 用例总数：42
- 方法类型：均为 `POST`
- 测试类型覆盖：
  - 正向（positive）：14
  - 负向（negative）：14
  - 边界（boundary）：14

## 2. 通用测试点提炼

### 2.1 协议与基础校验

- 请求方法与路径正确性校验（POST + 对应 endpoint）
- 请求头 `Content-Type: application/json` 校验
- 响应基础结构校验：`code`、`msg`、`data` 字段存在性与类型合理性
- 状态码/业务码一致性校验（正向 200、异常场景 400）

### 2.2 参数校验

- 必填参数缺失校验（如 `gimiDevice`、`systemVersion`、`versionCode`）
- 参数类型校验（如 `versionCode`、`beginning/ending`、`playerWidth/playerHeight`）
- 参数结构校验（如 `channelList` 需为对象数组）
- 可选参数兼容性校验（可不传、空值、空数组）

### 2.3 业务逻辑校验

- 过滤条件生效校验（频道 ID、来源、时间区间）
- 时间区间逻辑校验（`beginning == ending`、`beginning > ending`）
- 数据完整性校验（返回列表/详情关键字段）

### 2.4 健壮性与边界校验

- 数值边界（`versionCode=0`、`versionCode=int32_max`）
- 分辨率边界（`0x0`、`1x1`）
- 长字符串与特殊字符兼容性（`pn/deviceId/channelId/deviceMac`）
- 空数组输入稳定性（`channelIdList=[]`、`channelList=[]`）

## 3. 分接口测试点

## 3.1 获取fastchannel分类列表
- 接口：`/bff/video/v1/fastchannel/categories`
- 测试重点：
  - 必填参数最小集可成功返回分类数据
  - 全量参数输入时兼容设备信息扩展字段
  - 缺失必填、类型错误触发参数校验
  - `versionCode` 边界值与 `pn` 特殊字符输入稳定性

## 3.2 获取fastchannel媒资列表（v1）
- 接口：`/bff/video/v1/fastchannel/metas`
- 测试重点：
  - 必填参数可拉取媒资列表
  - `channelIdList + beginning/ending` 过滤逻辑正确
  - 缺少必填与时间参数类型错误的异常处理
  - 空频道数组、时间等值边界场景稳定性

## 3.3 获取fastchannel频道列表（v1）
- 接口：`/bff/video/v1/fastchannel/channels`
- 测试重点：
  - 必填/全量设备参数场景可正常返回频道列表
  - 必填缺失、类型错误校验有效
  - 超长字符串与特殊字符输入兼容性

## 3.4 获取设备唯一Id
- 接口：`/bff/video/v1/livetv/getAuid`
- 测试重点：
  - 必填参数可成功返回 `data.auid`
  - 全量参数下唯一 ID 返回稳定
  - 必填缺失、类型错误可被拦截
  - 空 `deviceId`、`versionCode` 上边界处理稳定

## 3.5 获取频道详情
- 接口：`/bff/video/v1/livetv/getChanelDetail`
- 测试重点：
  - 必填参数返回详情基础结构
  - 全量参数（含分辨率、频道 ID）返回目标频道详情
  - 必填缺失、分辨率类型错误拦截
  - 最小分辨率与特殊字符 `channelId` 兼容性

## 3.6 获取fastchannel媒资列表（v2）
- 接口：`/bff/video/v2/fastchannel/metas`
- 测试重点：
  - v2 结构下必填参数与全量参数正常流程
  - `channelList` 结构合法性校验（对象数组）
  - 空 `channelList` 边界稳定性
  - 反向时间区间业务校验（`beginning > ending`）

## 3.7 获取fastchannel频道列表（v2）
- 接口：`/bff/video/v2/fastchannel/channels`
- 测试重点：
  - 必填与全量参数正常返回频道集合
  - 必填缺失、类型错误异常处理
  - 分辨率边界（0 值）与 `deviceId` 特殊字符兼容

## 4. 覆盖度结论

- 当前用例已覆盖核心功能路径、关键参数校验、常见异常输入与主要边界场景。
- 对接口自动化落地友好，适合直接用于参数化执行（pytest + allure）。

## 5. 建议补充测试点（下一步）

- 鉴权与权限：未登录、token 失效、越权访问
- 错误码精细化：按接口真实错误码字典校准期望值
- 性能与稳定性：高并发、长稳压测、超时重试策略
- 数据一致性：跨接口联动（频道列表 -> 频道详情 -> 媒资列表）结果一致性
- 幂等与重复请求：相同参数重复调用结果稳定性
