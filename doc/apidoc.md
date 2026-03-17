 <h1 class="curproject-name"> 海外服务（C端） </h1> 
            
# fast-channel-controller

## 获取fastchannel分类列表

<a id=获取fastchannel分类列表> </a>

### 基本信息

**Path：** /bff/video/v1/fastchannel/categories

**Method：** POST

**接口描述：**
获取fastchannel分类列表

### 请求参数

**Headers**

| 参数名称     | 参数值           | 是否必须 | 示例 | 备注 |
| ------------ | ---------------- | -------- | ---- | ---- |
| Content-Type | application/json | 是       |      |      |

**Query**

| 参数名称      | 是否必须 | 示例 | 备注                                                    |
| ------------- | -------- | ---- | ------------------------------------------------------- |
| gimiPid       | 否       |      | 设备串号,sn                                             |
| gimiDevice    | 是       |      | 设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name |
| deviceMac     | 否       |      | 设备mac地址                                             |
| systemVersion | 是       |      | 系统版本号                                              |
| versionCode   | 是       |      | 应用版本号                                              |
| pn            | 否       |      | product name设备名称，安卓通用                          |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">plex返回数据</span></td><td key=5></td></tr><tr key=0-1-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> data</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">data</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-0-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">id</span></td><td key=5></td></tr><tr key=0-1-0-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">name名字</span></td><td key=5></td></tr><tr key=0-1-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> deviceMac</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">设备mac地址</span></td><td key=5></td></tr><tr key=0-1-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> gimiDevice</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name</span></td><td key=5></td></tr><tr key=0-1-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> gimiPid</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">设备串号,sn</span></td><td key=5></td></tr><tr key=0-1-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> pn</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"> product name设备名称，安卓通用</span></td><td key=5></td></tr><tr key=0-1-5><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> systemVersion</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">系统版本号</span></td><td key=5></td></tr><tr key=0-1-6><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> timezone</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">timezone</span></td><td key=5></td></tr><tr key=0-1-7><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> versionCode</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">应用版本号</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr>
               </tbody>
              </table>
            
## 获取fastchannel媒资列表
<a id=获取fastchannel媒资列表> </a>
### 基本信息

**Path：** /bff/video/v1/fastchannel/metas

**Method：** POST

**接口描述：**
获取fastchannel媒资列表

### 请求参数

**Headers**

| 参数名称     | 参数值           | 是否必须 | 示例 | 备注 |
| ------------ | ---------------- | -------- | ---- | ---- |
| Content-Type | application/json | 是       |      |      |

**Query**

| 参数名称      | 是否必须 | 示例 | 备注                                                    |
| ------------- | -------- | ---- | ------------------------------------------------------- |
| channelIdList | 否       |      | 分组id,tripartiteId                                     |
| gimiPid       | 否       |      | 设备串号,sn                                             |
| gimiDevice    | 是       |      | 设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name |
| deviceMac     | 否       |      | 设备mac地址                                             |
| systemVersion | 是       |      | 系统版本号                                              |
| versionCode   | 是       |      | 应用版本号                                              |
| pn            | 否       |      | product name设备名称，安卓通用                          |
| beginning     | 否       |      | 开始时间                                                |
| ending        | 否       |      | 结束时间                                                |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> channelId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">频道ID</span></td><td key=5></td></tr><tr key=0-1-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> metaDataList</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">媒资数据</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-1-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> beginning</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">beginning</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int64</span></p></td></tr><tr key=0-1-1-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> desc</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">desc描述</span></td><td key=5></td></tr><tr key=0-1-1-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> duration</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">duration时长，秒</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int64</span></p></td></tr><tr key=0-1-1-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> ending</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">ending</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int64</span></p></td></tr><tr key=0-1-1-4><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> episode</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">episode剧集信息</span></td><td key=5></td></tr><tr key=0-1-1-5><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> gmId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">id</span></td><td key=5></td></tr><tr key=0-1-1-6><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> icon</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">icon</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-1-6-0><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-6-1><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-1-6-2><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-1-6-3><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-1-6-4><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-7><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">name名字</span></td><td key=5></td></tr><tr key=0-1-1-8><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> poster</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">poster海报</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-1-8-0><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-8-1><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-1-8-2><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-1-8-3><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-1-8-4><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-9><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> publicationDate</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">publicationDate发布日期</span></td><td key=5></td></tr><tr key=0-1-1-10><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> showTime</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">showTime</span></td><td key=5></td></tr><tr key=0-1-1-11><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> tripartiteId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">tripartiteId</span></td><td key=5></td></tr><tr key=0-1-1-12><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> type</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">type类型</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr>
               </tbody>
              </table>
            
## 获取fastchannel频道列表
<a id=获取fastchannel频道列表> </a>
### 基本信息

**Path：** /bff/video/v1/fastchannel/channels

**Method：** POST

**接口描述：**
获取fastchannel频道列表

### 请求参数

**Headers**

| 参数名称     | 参数值           | 是否必须 | 示例 | 备注 |
| ------------ | ---------------- | -------- | ---- | ---- |
| Content-Type | application/json | 是       |      |      |

**Query**

| 参数名称      | 是否必须 | 示例 | 备注                                                    |
| ------------- | -------- | ---- | ------------------------------------------------------- |
| gimiPid       | 否       |      | 设备串号,sn                                             |
| gimiDevice    | 是       |      | 设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name |
| deviceMac     | 否       |      | 设备mac地址                                             |
| systemVersion | 是       |      | 系统版本号                                              |
| versionCode   | 是       |      | 应用版本号                                              |
| pn            | 否       |      | product name设备名称，安卓通用                          |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> categoryList</span></td><td key=1><span>string []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">categoryList分类</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>string</span></p></td></tr><tr key=array-74><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> </span></td><td key=1><span></span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> desc</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">desc</span></td><td key=5></td></tr><tr key=0-1-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> gmId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">id</span></td><td key=5></td></tr><tr key=0-1-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> icon</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">icon</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-3-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-3-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-3-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-3-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-3-4><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">name</span></td><td key=5></td></tr><tr key=0-1-5><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> poster</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">poster</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-5-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-5-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-5-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-5-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-5-4><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-6><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> source</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">source来源</span></td><td key=5></td></tr><tr key=0-1-7><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> tripartiteId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">tripartiteId</span></td><td key=5></td></tr><tr key=0-1-8><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">url打开地址</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr>
               </tbody>
              </table>
            
            
## 获取设备唯一Id
<a id=获取设备唯一Id> </a>
### 基本信息

**Path：** /bff/video/v1/livetv/getAuid

**Method：** POST

**接口描述：**
获取设备唯一Id

### 请求参数

**Headers**

| 参数名称     | 参数值           | 是否必须 | 示例 | 备注 |
| ------------ | ---------------- | -------- | ---- | ---- |
| Content-Type | application/json | 是       |      |      |

**Query**

| 参数名称      | 是否必须 | 示例 | 备注                                                    |
| ------------- | -------- | ---- | ------------------------------------------------------- |
| gimiPid       | 否       |      | 设备串号,sn                                             |
| gimiDevice    | 是       |      | 设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name |
| deviceMac     | 否       |      | 设备mac地址                                             |
| systemVersion | 是       |      | 系统版本号                                              |
| versionCode   | 是       |      | 应用版本号                                              |
| pn            | 否       |      | product name设备名称，安卓通用                          |
| deviceId      | 否       |      | 设备唯一标识                                            |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> auid</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr>
               </tbody>
              </table>
            
            
## 获取频道详情
<a id=获取频道详情> </a>
### 基本信息

**Path：** /bff/video/v1/livetv/getChanelDetail

**Method：** POST

**接口描述：**
获取频道详情

### 请求参数

**Headers**

| 参数名称     | 参数值           | 是否必须 | 示例 | 备注 |
| ------------ | ---------------- | -------- | ---- | ---- |
| Content-Type | application/json | 是       |      |      |

**Query**

| 参数名称      | 是否必须 | 示例 | 备注                                                    |
| ------------- | -------- | ---- | ------------------------------------------------------- |
| gimiPid       | 否       |      | 设备串号,sn                                             |
| gimiDevice    | 是       |      | 设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name |
| deviceMac     | 否       |      | 设备mac地址                                             |
| systemVersion | 是       |      | 系统版本号                                              |
| versionCode   | 是       |      | 应用版本号                                              |
| pn            | 否       |      | product name设备名称，安卓通用                          |
| deviceId      | 否       |      | 设备唯一标识                                            |
| playerWidth   | 否       |      | 播放器分辨率-宽度                                       |
| playerHeight  | 否       |      | 播放器分辨率-高度                                       |
| channelId     | 否       |      | 频道Id                                                  |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> anokiChannel</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> channelId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> createNewDrmSession</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> genre</span></td><td key=1><span>string []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>string</span></p></td></tr><tr key=array-78><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> </span></td><td key=1><span></span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> logo</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-5><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-6><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> playbackUrl</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-7><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> rating</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-8><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> resolution</span></td><td key=1><span>string []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>string</span></p></td></tr><tr key=array-79><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> </span></td><td key=1><span></span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr>
               </tbody>
              </table>
            
# fast-channel-v-2-controller

## 获取fastchannel媒资列表

<a id=获取fastchannel媒资列表> </a>

### 基本信息

**Path：** /bff/video/v2/fastchannel/metas

**Method：** POST

**接口描述：**
获取fastchannel媒资列表

### 请求参数

**Headers**

| 参数名称     | 参数值           | 是否必须 | 示例 | 备注 |
| ------------ | ---------------- | -------- | ---- | ---- |
| Content-Type | application/json | 是       |      |      |

**Query**

| 参数名称                 | 是否必须 | 示例 | 备注                                                    |
| ------------------------ | -------- | ---- | ------------------------------------------------------- |
| channelList[0].channelId | 否       |      | 频道id                                                  |
| channelList[0].source    | 否       |      | 来源                                                    |
| gimiPid                  | 否       |      | 设备串号,sn                                             |
| gimiDevice               | 是       |      | 设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name |
| deviceMac                | 否       |      | 设备mac地址                                             |
| systemVersion            | 是       |      | 系统版本号                                              |
| versionCode              | 是       |      | 应用版本号                                              |
| pn                       | 否       |      | product name设备名称，安卓通用                          |
| deviceId                 | 否       |      | 设备id                                                  |
| beginning                | 否       |      | 开始时间                                                |
| ending                   | 否       |      | 结束时间                                                |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> channelId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">频道ID</span></td><td key=5></td></tr><tr key=0-1-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> metaDataList</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">媒资数据</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-1-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> beginning</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">beginning</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int64</span></p></td></tr><tr key=0-1-1-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> desc</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">desc描述</span></td><td key=5></td></tr><tr key=0-1-1-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> duration</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">duration时长，秒</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int64</span></p></td></tr><tr key=0-1-1-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> ending</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">ending</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int64</span></p></td></tr><tr key=0-1-1-4><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> episode</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">episode剧集信息</span></td><td key=5></td></tr><tr key=0-1-1-5><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> gmId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">id</span></td><td key=5></td></tr><tr key=0-1-1-6><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> icon</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">icon</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-1-6-0><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-6-1><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-1-6-2><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-1-6-3><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-1-6-4><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-7><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">name名字</span></td><td key=5></td></tr><tr key=0-1-1-8><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> poster</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">poster海报</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-1-8-0><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-8-1><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-1-8-2><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-1-8-3><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-1-8-4><td key=0><span style="padding-left: 60px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-1-9><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> publicationDate</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">publicationDate发布日期</span></td><td key=5></td></tr><tr key=0-1-1-10><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> showTime</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">showTime</span></td><td key=5></td></tr><tr key=0-1-1-11><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> tripartiteId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">tripartiteId</span></td><td key=5></td></tr><tr key=0-1-1-12><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> type</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">type类型</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr>
               </tbody>
              </table>
            
## 获取fastchannel频道列表
<a id=获取fastchannel频道列表> </a>
### 基本信息

**Path：** /bff/video/v2/fastchannel/channels

**Method：** POST

**接口描述：**
获取fastchannel频道列表

### 请求参数

**Headers**

| 参数名称     | 参数值           | 是否必须 | 示例 | 备注 |
| ------------ | ---------------- | -------- | ---- | ---- |
| Content-Type | application/json | 是       |      |      |

**Query**

| 参数名称      | 是否必须 | 示例 | 备注                                                    |
| ------------- | -------- | ---- | ------------------------------------------------------- |
| gimiPid       | 否       |      | 设备串号,sn                                             |
| gimiDevice    | 是       |      | 设备名称，确定唯一机型,使用ro_vendor_xgimi_product_name |
| deviceMac     | 否       |      | 设备mac地址                                             |
| systemVersion | 是       |      | 系统版本号                                              |
| versionCode   | 是       |      | 应用版本号                                              |
| pn            | 否       |      | product name设备名称，安卓通用                          |
| deviceId      | 否       |      | 设备唯一标识                                            |
| playerWidth   | 否       |      | 播放器分辨率-宽度                                       |
| playerHeight  | 否       |      | 播放器分辨率-高度                                       |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>integer</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> categoryList</span></td><td key=1><span>string []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">categoryList分类</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>string</span></p></td></tr><tr key=array-80><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> </span></td><td key=1><span></span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> desc</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">desc</span></td><td key=5></td></tr><tr key=0-1-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> gmId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">id</span></td><td key=5></td></tr><tr key=0-1-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> icon</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">icon</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-3-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-3-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-3-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-3-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-3-4><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">name</span></td><td key=5></td></tr><tr key=0-1-5><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> poster</span></td><td key=1><span>object []</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">poster</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-1-5-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> height</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">高</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-5-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> orientation</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">方向，枚举：“LANDSCAPE”、“PORTRAIT” </span></td><td key=5></td></tr><tr key=0-1-5-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> original</span></td><td key=1><span>boolean</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-1-5-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">图片地址</span></td><td key=5></td></tr><tr key=0-1-5-4><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> width</span></td><td key=1><span>integer</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">宽</span></td><td key=5><p key=2><span style="font-weight: '700'">format: </span><span>int32</span></p></td></tr><tr key=0-1-6><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> source</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">source来源</span></td><td key=5></td></tr><tr key=0-1-7><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> tripartiteId</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">tripartiteId</span></td><td key=5></td></tr><tr key=0-1-8><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> url</span></td><td key=1><span>string</span></td><td key=2>非必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">url打开地址</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr>
               </tbody>
              </table>
