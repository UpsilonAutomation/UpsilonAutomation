# Interface IFBoxClientManager

盒子系统客户端接口

#### Inherited Members

System.IDisposable.Dispose\(\)

**Namespace: FBoxClientDriver.Contract**

**Assembly: FBoxClientDriver.Contract.dll**

#### Syntax <a id="FBoxClientDriver_Contract_IFBoxClientManager_syntax"></a>

```text
public interface IFBoxClientManager : IDisposable
```

## Methods <a id="methods"></a>

### AddAlarmDefinitionV2\(AddAlarmDefArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddAlarmDefinitionV2_FBoxClientDriver_Contract_AddAlarmDefArgsV2_"></a>

新增报警监控条目V2（支持离线编辑）

#### Declaration

```text
Task> AddAlarmDefinitionV2(AddAlarmDefArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddAlarmDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddAlarmDefArgsV2.html) | args | 新增报警条目参数[AddAlarmDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddAlarmDefArgsV2.html)报警条目参数 |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;System.Int64&gt;&gt; | 返回报警条目ID集合 |

### AddAlarmDefiniton\(AddAlarmDefinitonArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddAlarmDefiniton_FBoxClientDriver_Contract_AddAlarmDefinitonArgs_"></a>

新增报警条目

#### Declaration

```text
[Obsolete]
Task AddAlarmDefiniton(AddAlarmDefinitonArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddAlarmDefinitonArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddAlarmDefinitonArgs.html) | args | 新增报警条目参数[AddAlarmDefinitonArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddAlarmDefinitonArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; | 新增报警条目的UID |

### AddAlarmGroup\(AddAlarmGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddAlarmGroup_FBoxClientDriver_Contract_AddAlarmGroupArgs_"></a>

增加报警分组

#### Declaration

```text
Task AddAlarmGroup(AddAlarmGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddAlarmGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddAlarmGroupArgs.html) | args | 报警分组参数[AddAlarmGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddAlarmGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; | 新增报警分组UID |

### AddAlarmTarget\(AddTargetArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddAlarmTarget_FBoxClientDriver_Contract_AddTargetArgs_"></a>

增加报警联系人

#### Declaration

```text
Task AddAlarmTarget(AddTargetArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddTargetArgs.html) | args | 新增报警联系人参数[AddTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddTargetArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; | 报警联系人Id |

### AddBoxGroup\(AddBoxGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddBoxGroup_FBoxClientDriver_Contract_AddBoxGroupArgs_"></a>

新增盒子分组

#### Declaration

```text
Task AddBoxGroup(AddBoxGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddBoxGroupArgs.html) | args | 要新增盒子分组的参数信息[AddBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddBoxGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; | 新增盒子组别的UID |

### AddDataMonitorGroup\(AddDataMonitorGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddDataMonitorGroup_FBoxClientDriver_Contract_AddDataMonitorGroupArgs_"></a>

增加监控点组

#### Declaration

```text
Task AddDataMonitorGroup(AddDataMonitorGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddDataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDataMonitorGroupArgs.html) | args | 新增监测点组别参数[AddDataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDataMonitorGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; | 新增监测点的UID |

### AddDataMonitorPoint\(AddDataMonitorDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddDataMonitorPoint_FBoxClientDriver_Contract_AddDataMonitorDefinitionArgs_"></a>

增加监控点条目

#### Declaration

```text
[Obsolete]
Task AddDataMonitorPoint(AddDataMonitorDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddDataMonitorDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDataMonitorDefinitionArgs.html) | args | 新增监测点信息参数[AddDataMonitorDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDataMonitorDefinitionArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; | 新增监测点的UID |

### AddDataMonitorPointV2\(AddDmonsArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddDataMonitorPointV2_FBoxClientDriver_Contract_AddDmonsArgsV2_"></a>

新增监控点条目V2\(支持离线编辑\),集合长度不要超过20个

#### Declaration

```text
Task> AddDataMonitorPointV2(AddDmonsArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddDmonsArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDmonsArgsV2.html) | args | 新增监控点参数[AddDmonsArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddDmonsArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;System.Int64&gt;&gt; | 返回监控点ID集合 |

### AddHdataDefinitionV2\(AddHdataDefArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddHdataDefinitionV2_FBoxClientDriver_Contract_AddHdataDefArgsV2_"></a>

新增历史记录条目

#### Declaration

```text
[Obsolete]
Task> AddHdataDefinitionV2(AddHdataDefArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddHdataDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataDefArgsV2.html) | args | 新增历史记录条目参数[AddHdataDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataDefArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;System.Int64&gt;&gt; | 历史记录id集合 |

### AddHdataItems\(AddHdataItemArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddHdataItems_FBoxClientDriver_Contract_AddHdataItemArgs_"></a>

新增历史记录多通道

#### Declaration

```text
Task> AddHdataItems(AddHdataItemArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddHdataItemArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataItemArgs.html) | args | 新增历史记录多通道参数[AddHdataItemArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHdataItemArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;System.Int64&gt;&gt; | System.Int64 |

### AddHistoryDefinition\(AddHDataDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_AddHistoryDefinition_FBoxClientDriver_Contract_AddHDataDefinitionArgs_"></a>

新增历史记录条目

#### Declaration

```text
[Obsolete]
Task AddHistoryDefinition(AddHDataDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddHDataDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHDataDefinitionArgs.html) | args | 新增历史监控点参数 [AddHDataDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddHDataDefinitionArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; | 历史条目id |

### ChangeBoxGroup\(ChangeBoxGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_ChangeBoxGroup_FBoxClientDriver_Contract_ChangeBoxGroupArgs_"></a>

更换盒子分组

#### Declaration

```text
Task ChangeBoxGroup(ChangeBoxGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [ChangeBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ChangeBoxGroupArgs.html) | args | 要更换盒子分组的参数信息 [ChangeBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ChangeBoxGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### ChangeBoxOwner\(ChangeBoxOwnerArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_ChangeBoxOwner_FBoxClientDriver_Contract_ChangeBoxOwnerArgsV2_"></a>

移交盒子

#### Declaration

```text
Task ChangeBoxOwner(ChangeBoxOwnerArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [ChangeBoxOwnerArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ChangeBoxOwnerArgsV2.html) | args | 移交盒子参数[ChangeBoxOwnerArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ChangeBoxOwnerArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### CheckBoxIsBelongs\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_CheckBoxIsBelongs_FBoxClientDriver_Contract_BoxArgs_"></a>

校验盒子是否属于自己

#### Declaration

```text
Task CheckBoxIsBelongs(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Boolean&gt; | bool |

### Clean\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_Clean"></a>

清除已经登录的用户信息，方便重新登录

#### Declaration

### ConfirmAlarm\(AlarmConfirmArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_ConfirmAlarm_FBoxClientDriver_Contract_AlarmConfirmArgs_"></a>

确认报警

#### Declaration

```text
Task ConfirmAlarm(AlarmConfirmArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AlarmConfirmArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConfirmArgs.html) | args | 确认报警参数[AlarmConfirmArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConfirmArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### ConnectBoxSignalR\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_ConnectBoxSignalR"></a>

#### Declaration

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### ConnectMainSignalR\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_ConnectMainSignalR"></a>

#### Declaration

```text
Task ConnectMainSignalR()
```

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### DownLoadPlcs\(DownLoadPlcArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_DownLoadPlcs_FBoxClientDriver_Contract_DownLoadPlcArgs_"></a>

下载PLC

#### Declaration

```text
Task DownLoadPlcs(DownLoadPlcArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DownLoadPlcArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DownLoadPlcArgs.html) | args | 下载PLC参数 [DownLoadPlcArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DownLoadPlcArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### DownLoadPlcsRestart\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_DownLoadPlcsRestart_FBoxClientDriver_Contract_BoxArgs_"></a>

下载PLC后重启FBox

#### Declaration

```text
Task DownLoadPlcsRestart(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### DownLoadPlcsV2\(AddOrUpdatePlcDeviceArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_DownLoadPlcsV2_FBoxClientDriver_Contract_AddOrUpdatePlcDeviceArgsV2_"></a>

下载PLC V2\(支持离线下载\)

#### Declaration

```text
Task DownLoadPlcsV2(AddOrUpdatePlcDeviceArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AddOrUpdatePlcDeviceArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddOrUpdatePlcDeviceArgsV2.html) | args | 下载的驱动列表 [AddOrUpdatePlcDeviceArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AddOrUpdatePlcDeviceArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### ExportHistoryDataCsv\(ExportHistoryDataCsvArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_ExportHistoryDataCsv_FBoxClientDriver_Contract_ExportHistoryDataCsvArgs_"></a>

导出历史记录文件\(CSV\)

#### Declaration

```text
Task ExportHistoryDataCsv(ExportHistoryDataCsvArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [ExportHistoryDataCsvArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ExportHistoryDataCsvArgs.html) | args | [ExportHistoryDataCsvArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.ExportHistoryDataCsvArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.IO.Stream&gt; |  |

### GetAlarmEvents\(AlarmEventQuery\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAlarmEvents_FBoxClientDriver_Contract_AlarmEventQuery_"></a>

获取报警历史记录

#### Declaration

```text
Task> GetAlarmEvents(AlarmEventQuery args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AlarmEventQuery](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmEventQuery.html) | args | 查询报警历史记录参数[AlarmEventQuery](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmEventQuery.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[AlarmEvent](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmEvent.html)&gt;&gt; | 报警历史记录列表[AlarmEvent](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmEvent.html) |

### GetAlarmEvents2\(AlarmEventQuery2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAlarmEvents2_FBoxClientDriver_Contract_AlarmEventQuery2_"></a>

#### Declaration

```text
Task> GetAlarmEvents2(AlarmEventQuery2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [AlarmEventQuery2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmEventQuery2.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[AlarmEvent](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmEvent.html)&gt;&gt; |  |

### GetAlarmGroups\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAlarmGroups_FBoxClientDriver_Contract_BoxArgs_"></a>

获取所有报警分组

#### Declaration

```text
Task> GetAlarmGroups(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子信息参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[AlarmGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmGroup.html)&gt;&gt; | 报警组别列表[AlarmGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmGroup.html) |

### GetAlarmMonitorDefiniton\(GetAlarmDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAlarmMonitorDefiniton_FBoxClientDriver_Contract_GetAlarmDefinitionArgs_"></a>

获取报警条目

#### Declaration

```text
[Obsolete]
Task GetAlarmMonitorDefiniton(GetAlarmDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetAlarmDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetAlarmDefinitionArgs.html) | args | 获取报警条目参数[GetAlarmDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetAlarmDefinitionArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[AlarmMonitorDefinition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmMonitorDefinition.html)&gt; | 报警条目信息[AlarmMonitorDefinition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmMonitorDefinition.html) |

### GetAlarmMonitorDefintions\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAlarmMonitorDefintions_FBoxClientDriver_Contract_BoxArgs_"></a>

获取报警条目列表

#### Declaration

```text
Task> GetAlarmMonitorDefintions(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子信息参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[AlarmMonitorDefinition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmMonitorDefinition.html)&gt;&gt; | 报警条目列表[AlarmMonitorDefinition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmMonitorDefinition.html) |

### GetAlarmTarget\(GetAlarmTargetArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAlarmTarget_FBoxClientDriver_Contract_GetAlarmTargetArgs_"></a>

获取报警联系人

#### Declaration

```text
Task GetAlarmTarget(GetAlarmTargetArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetAlarmTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetAlarmTargetArgs.html) | args | 获取报警联系人参数[GetAlarmTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetAlarmTargetArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[AlarmTarget](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmTarget.html)&gt; | 报警联系人[AlarmTarget](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmTarget.html) |

### GetAlarmTargets\(GetAlarmTargetsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAlarmTargets_FBoxClientDriver_Contract_GetAlarmTargetsArgs_"></a>

获取报警联系人列表

#### Declaration

```text
Task> GetAlarmTargets(GetAlarmTargetsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetAlarmTargetsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetAlarmTargetsArgs.html) | args | 获取报警联系人列表参数[GetAlarmTargetsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetAlarmTargetsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[AlarmTarget](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmTarget.html)&gt;&gt; | 报警联系人列表[AlarmTarget](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmTarget.html) |

### GetAllAlarmDefinitionsV2\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetAllAlarmDefinitionsV2_FBoxClientDriver_Contract_BoxArgs_"></a>

获取盒子底下所有的报警条目

#### Declaration

```text
Task> GetAllAlarmDefinitionsV2(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子参数 |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[AlarmDefintitionDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmDefintitionDtoV2.html)&gt;&gt; | 报警条目列表[AlarmDefintitionDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmDefintitionDtoV2.html) |

### GetBox\(GetBoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBox_FBoxClientDriver_Contract_GetBoxArgs_"></a>

获取单个盒子注册信息

#### Declaration

```text
Task GetBox(GetBoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetBoxArgs.html) | args | 获取盒子信息参数[GetBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetBoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[Box](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Box.html)&gt; | 盒子信息[Box](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Box.html) |

### GetBoxAlarmEventObservable\(BoxCollectionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxAlarmEventObservable_FBoxClientDriver_Contract_BoxCollectionArgs_"></a>

#### Declaration

```text
IObservable> GetBoxAlarmEventObservable(BoxCollectionArgs boxes)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxCollectionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxCollectionArgs.html) | boxes |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.IObservable&lt;System.Collections.Generic.IList&lt;[BoxAlarmEvent](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxAlarmEvent.html)&gt;&gt; |  |

### GetBoxDeviceList\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxDeviceList_FBoxClientDriver_Contract_BoxArgs_"></a>

根据盒子编码获取盒子设备列表

#### Declaration

```text
[Obsolete]
Task> GetBoxDeviceList(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子信息参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[BoxDeviceInfo](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxDeviceInfo.html)&gt;&gt; | 盒子设备信息列表[BoxDeviceInfo](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxDeviceInfo.html) |

### GetBoxGroup\(GetBoxGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxGroup_FBoxClientDriver_Contract_GetBoxGroupArgs_"></a>

根据盒子组别UID获取盒子组别

#### Declaration

```text
Task GetBoxGroup(GetBoxGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetBoxGroupArgs.html) | args | 获取盒子组别信息参数[GetBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetBoxGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[BoxGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxGroup.html)&gt; | 盒子组别[BoxGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxGroup.html) |

### GetBoxGroups\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxGroups"></a>

获取盒子分组和盒子信息

#### Declaration

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[BoxGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxGroup.html)&gt;&gt; | 盒子组别列表[BoxGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxGroup.html) |

### GetBoxLocations\(GetLocationArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxLocations_FBoxClientDriver_Contract_GetLocationArgs_"></a>

获取盒子地理未知

#### Declaration

```text
Task> GetBoxLocations(GetLocationArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetLocationArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetLocationArgs.html) | args | [GetLocationArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetLocationArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[BoxLocation](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.BoxLocation.html)&gt;&gt; | [BoxLocation](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.BoxLocation.html) |

### GetBoxs\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxs"></a>

获取该用户下的所有盒子列表

#### Declaration

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[Box](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Box.html)&gt;&gt; | 用户下的盒子列表[Box](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Box.html) |

### GetBoxState\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxState"></a>

获取盒子状态

#### Declaration

#### Returns

| Type | Description |
| :--- | :--- |
| System.Collections.Generic.IList&lt;[BoxStateEntity](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxStateEntity.html)&gt; | [BoxStateEntity](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxStateEntity.html) |

### GetBoxStateChangedObservable\(BoxCollectionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxStateChangedObservable_FBoxClientDriver_Contract_BoxCollectionArgs_"></a>

#### Declaration

```text
IObservable> GetBoxStateChangedObservable(BoxCollectionArgs boxes)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxCollectionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxCollectionArgs.html) | boxes |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.IObservable&lt;System.Collections.Generic.IList&lt;[BoxStateChangedEvent](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxStateChangedEvent.html)&gt;&gt; |  |

### GetBoxType\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetBoxType_FBoxClientDriver_Contract_BoxArgs_"></a>

获取盒子类型

#### Declaration

```text
Task GetBoxType(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[BoxTypes](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxTypes.html)&gt; |  |

### GetByChannelHistoryData\(GetHistoryDataArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetByChannelHistoryData_FBoxClientDriver_Contract_GetHistoryDataArgs_"></a>

获取历史记录多通道曲线数据

#### Declaration

```text
Task GetByChannelHistoryData(GetHistoryDataArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetHistoryDataArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetHistoryDataArgs.html) | args | [GetHistoryDataArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetHistoryDataArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[ByChannelHistoryData](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.ByChannelHistoryData.html)&gt; |  |

### GetByRowHistoryData\(GetHistoryDataArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetByRowHistoryData_FBoxClientDriver_Contract_GetHistoryDataArgs_"></a>

获取历史记录多通道数据

#### Declaration

```text
Task GetByRowHistoryData(GetHistoryDataArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetHistoryDataArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetHistoryDataArgs.html) | args | [GetHistoryDataArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetHistoryDataArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[ByRowHistoryData](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.ByRowHistoryData.html)&gt; | [ByRowHistoryData](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.ByRowHistoryData.html) |

### GetCellLocation\(Int32, Int32, Int32, Int32\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetCellLocation_System_Int32_System_Int32_System_Int32_System_Int32_"></a>

获取基站地理位置信息（WGS84格式）

#### Declaration

```text
Task GetCellLocation(int mcc, int mnc, int lac, int ci)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| System.Int32 | mcc |  |
| System.Int32 | mnc |  |
| System.Int32 | lac |  |
| System.Int32 | ci |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[CellLocationResult](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.CellLocationResult.html)&gt; |  |

### GetDataMonitorDefiniton\(GetDataMonitorDefArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDataMonitorDefiniton_FBoxClientDriver_Contract_GetDataMonitorDefArgs_"></a>

获取单条监测点条目

#### Declaration

```text
[Obsolete]
Task GetDataMonitorDefiniton(GetDataMonitorDefArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetDataMonitorDefArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDataMonitorDefArgs.html) | args | 获取监测点信息参数[GetDataMonitorDefArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDataMonitorDefArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[DataMonitorDefinition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorDefinition.html)&gt; | 空 |

### GetDataMonitorGroup\(GetDMonitorGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDataMonitorGroup_FBoxClientDriver_Contract_GetDMonitorGroupArgs_"></a>

获取监控点分组

#### Declaration

```text
Task GetDataMonitorGroup(GetDMonitorGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetDMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDMonitorGroupArgs.html) | args | 获取监测点组别信息参数[GetDMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDMonitorGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[DataMonitorGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroup.html)&gt; | 监测点组别信息[DataMonitorGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroup.html) |

### GetDataMonitorGroups\(GetDMonitorGroupsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDataMonitorGroups_FBoxClientDriver_Contract_GetDMonitorGroupsArgs_"></a>

获取指定盒子上的监控点组列表

#### Declaration

```text
Task> GetDataMonitorGroups(GetDMonitorGroupsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetDMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDMonitorGroupsArgs.html) | args | 获取监测点组别列表参数[GetDMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDMonitorGroupsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[DataMonitorGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroup.html)&gt;&gt; | 检测点组别信息列表[DataMonitorGroup](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroup.html) |

### GetDevicePlcByBoxType\(BoxType\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDevicePlcByBoxType_FBoxClientDriver_Contract_BoxType_"></a>

获取盒子支持的所有PLC列表

#### Declaration

```text
Task> GetDevicePlcByBoxType(BoxType boxType)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxType.html) | boxType | 盒子类型[BoxType](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxType.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[PlcDevice](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcDevice.html)&gt;&gt; | PLC列表[PlcDevice](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcDevice.html) |

### GetDeviceSpecification\(GetDeviceSpecificationArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDeviceSpecification_FBoxClientDriver_Contract_GetDeviceSpecificationArgs_"></a>

根据设备ID获取所有设备信息

#### Declaration

```text
Task GetDeviceSpecification(GetDeviceSpecificationArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetDeviceSpecificationArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDeviceSpecificationArgs.html) | args | 获取设备信息参数[GetDeviceSpecificationArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDeviceSpecificationArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[DeviceSpecification](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceSpecification.html)&gt; | HMI等设备的规格信息[DeviceSpecification](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceSpecification.html) |

### GetDeviceSpecifications\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDeviceSpecifications"></a>

获取盒子支持的PLC/HMI等设备的规格信息

#### Declaration

```text
Task> GetDeviceSpecifications()
```

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[DeviceSpecification](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceSpecification.html)&gt;&gt; | PLC/HMI等设备的规格信息列表[DeviceSpecification](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DeviceSpecification.html) |

### GetDmonDataSouceId\(GetDmonDataSourceIdArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDmonDataSouceId_FBoxClientDriver_Contract_GetDmonDataSourceIdArgs_"></a>

根据监控点ID获取下发条目的实际Id

#### Declaration

```text
Task GetDmonDataSouceId(GetDmonDataSourceIdArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetDmonDataSourceIdArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDmonDataSourceIdArgs.html) | args | 获取Id参数 [GetDmonDataSourceIdArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDmonDataSourceIdArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int32&gt; |  |

### GetDmonGroupDmonsV2\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDmonGroupDmonsV2_FBoxClientDriver_Contract_BoxArgs_"></a>

获取盒子监控点分组与监控点条目

#### Declaration

```text
Task> GetDmonGroupDmonsV2(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子参数 |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[BoxDMonGroupsDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxDMonGroupsDtoV2.html)&gt;&gt; |  |

### GetDMonValue\(GetDMonValueArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetDMonValue_FBoxClientDriver_Contract_GetDMonValueArgs_"></a>

获取实时数据

#### Declaration

```text
Task> GetDMonValue(GetDMonValueArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetDMonValueArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDMonValueArgs.html) | args | 获取监控点数据参数[GetDMonValueArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetDMonValueArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[DMonEntry](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonEntry.html)&gt;&gt; | 返回数据列表[DMonEntry](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonEntry.html) |

### GetHdataDefinitionsV2\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetHdataDefinitionsV2_FBoxClientDriver_Contract_BoxArgs_"></a>

获取所有历史的记录条目

#### Declaration

```text
[Obsolete]
Task> GetHdataDefinitionsV2(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HdataDefinitionDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HdataDefinitionDtoV2.html)&gt;&gt; | 历史记录列表[HdataDefinitionDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HdataDefinitionDtoV2.html) |

### GetHdataItems\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetHdataItems_FBoxClientDriver_Contract_BoxArgs_"></a>

获取历史记录条目

#### Declaration

```text
Task> GetHdataItems(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HdataItem](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.HdataItem.html)&gt;&gt; | [HdataItem](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.HdataItem.html) |

### GetHistoryData\(HistoryDataQuery\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetHistoryData_FBoxClientDriver_Contract_HistoryDataQuery_"></a>

获取单个历史条目数据

#### Declaration

```text
[Obsolete]
Task> GetHistoryData(HistoryDataQuery args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [HistoryDataQuery](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HistoryDataQuery.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HistoryDataV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HistoryDataV2.html)&gt;&gt; |  |

### GetHistoryData2\(HistoryDataQuery2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetHistoryData2_FBoxClientDriver_Contract_HistoryDataQuery2_"></a>

获取多个历史条目数据

#### Declaration

```text
[Obsolete]
Task> GetHistoryData2(HistoryDataQuery2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [HistoryDataQuery2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HistoryDataQuery2.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HistoryDataV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HistoryDataV2.html)&gt;&gt; |  |

### GetHistoryDataList\(GetHDataArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetHistoryDataList_FBoxClientDriver_Contract_GetHDataArgs_"></a>

获取历史记录原始数据

#### Declaration

```text
[Obsolete]
Task> GetHistoryDataList(GetHDataArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetHDataArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetHDataArgs.html) | args | 获取历史记录参数[GetHDataArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetHDataArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HistoryData](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HistoryData.html)&gt;&gt; | 数据集合[HistoryData](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HistoryData.html) |

### GetHistoryItemDefinitions\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetHistoryItemDefinitions_FBoxClientDriver_Contract_BoxArgs_"></a>

获取历史记录条目列表

#### Declaration

```text
[Obsolete]
Task> GetHistoryItemDefinitions(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子信息参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HistoryItemDefinition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HistoryItemDefinition.html)&gt;&gt; | 空 |

### GetPlcDeviceV2\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetPlcDeviceV2_FBoxClientDriver_Contract_BoxArgs_"></a>

获取盒子下所有的PLC V2

#### Declaration

```text
Task> GetPlcDeviceV2(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 获取盒子PLC数据 |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[PlcDeviceDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcDeviceDtoV2.html)&gt;&gt; | [PlcDeviceDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcDeviceDtoV2.html)PLC驱动设备列表 |

### GetPlcs\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetPlcs"></a>

获取所有的PLC

#### Declaration

```text
[Obsolete]
Task GetPlcs()
```

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[PlcEntity](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcEntity.html)&gt; | PLC信息[PlcEntity](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.PlcEntity.html) |

### GetPositionInfo\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetPositionInfo_FBoxClientDriver_Contract_BoxArgs_"></a>

获取位置信息

#### Declaration

```text
[Obsolete]
Task GetPositionInfo(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子信息[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;[BoxPosition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxPosition.html)&gt; | 位置信息[BoxPosition](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxPosition.html) |

### GetRefreshTimeConfig\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetRefreshTimeConfig_FBoxClientDriver_Contract_BoxArgs_"></a>

获取盒子数据条目刷新时间（盒子全局设置）

#### Declaration

```text
Task GetRefreshTimeConfig(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int32&gt; | 刷新时间 |

### GetSomeAlarmDefinitionDtosV2\(GetSomeAlarmArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetSomeAlarmDefinitionDtosV2_FBoxClientDriver_Contract_GetSomeAlarmArgsV2_"></a>

获取某些报警条目信息V2

#### Declaration

```text
Task> GetSomeAlarmDefinitionDtosV2(GetSomeAlarmArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetSomeAlarmArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetSomeAlarmArgsV2.html) | args | 获取条目参数[GetSomeAlarmArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetSomeAlarmArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[AlarmDefintitionDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmDefintitionDtoV2.html)&gt;&gt; | 报警条目列表[AlarmDefintitionDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmDefintitionDtoV2.html) |

### GetSomeDmonsV2\(GetSomeDmonItemsArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetSomeDmonsV2_FBoxClientDriver_Contract_GetSomeDmonItemsArgsV2_"></a>

获取某些监控点条目信息

#### Declaration

```text
Task> GetSomeDmonsV2(GetSomeDmonItemsArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetSomeDmonItemsArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetSomeDmonItemsArgsV2.html) | args | 获取某些监控点参数 |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[DmonItemDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DmonItemDtoV2.html)&gt;&gt; |  |

### GetSomeHdataDefinitionV2\(GetSomeHdataArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetSomeHdataDefinitionV2_FBoxClientDriver_Contract_GetSomeHdataArgsV2_"></a>

获取某些历史的记录条目

#### Declaration

```text
[Obsolete]
Task> GetSomeHdataDefinitionV2(GetSomeHdataArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetSomeHdataArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetSomeHdataArgsV2.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HdataDefinitionDtoV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.HdataDefinitionDtoV2.html)&gt;&gt; |  |

### GetSomeHdataItems\(GetSomeHdataItemArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_GetSomeHdataItems_FBoxClientDriver_Contract_GetSomeHdataItemArgs_"></a>

获取某些历史记录条目

#### Declaration

```text
Task> GetSomeHdataItems(GetSomeHdataItemArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [GetSomeHdataItemArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetSomeHdataItemArgs.html) | args | 获取某些历史记录条目参数[GetSomeHdataItemArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.GetSomeHdataItemArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Collections.Generic.IList&lt;[HdataItem](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.HdataItem.html)&gt;&gt; | [HdataItem](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.Entity.HdataItem.html) |

### RebootBox\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RebootBox_FBoxClientDriver_Contract_BoxArgs_"></a>

重启盒子

#### Declaration

```text
Task RebootBox(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 要重启的盒子参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RegisterBox\(RegisterBoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RegisterBox_FBoxClientDriver_Contract_RegisterBoxArgs_"></a>

注册盒子

#### Declaration

```text
Task RegisterBox(RegisterBoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RegisterBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RegisterBoxArgs.html) | args | 要注册的盒子参数[RegisterBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RegisterBoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task&lt;System.Int64&gt; |  |

### RemoveAlarmDefinition\(RemoveAlarmDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveAlarmDefinition_FBoxClientDriver_Contract_RemoveAlarmDefinitionArgs_"></a>

删除报警条目

#### Declaration

```text
[Obsolete]
Task RemoveAlarmDefinition(RemoveAlarmDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveAlarmDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveAlarmDefinitionArgs.html) | args | 删除报警条目参数[RemoveAlarmDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveAlarmDefinitionArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveAlarmDefinitionV2\(RemoveAlarmDefArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveAlarmDefinitionV2_FBoxClientDriver_Contract_RemoveAlarmDefArgsV2_"></a>

删除报警监控点条目V2（支持离线编辑）

#### Declaration

```text
Task RemoveAlarmDefinitionV2(RemoveAlarmDefArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveAlarmDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveAlarmDefArgsV2.html) | args | 删除的报警点列表 |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveAlarmGroup\(RemoveAlarmGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveAlarmGroup_FBoxClientDriver_Contract_RemoveAlarmGroupArgs_"></a>

移除报警分组

#### Declaration

```text
Task RemoveAlarmGroup(RemoveAlarmGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveAlarmGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveAlarmGroupArgs.html) | args | 移除报警分组参数[RemoveAlarmGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveAlarmGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveAlarmTarget\(RemoveTargetArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveAlarmTarget_FBoxClientDriver_Contract_RemoveTargetArgs_"></a>

删除报警联系人

#### Declaration

```text
Task RemoveAlarmTarget(RemoveTargetArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveTargetArgs.html) | args | 移除报警联系人参数[RemoveTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveTargetArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveBoxGroup\(RemoveBoxGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveBoxGroup_FBoxClientDriver_Contract_RemoveBoxGroupArgs_"></a>

移除盒子分组

#### Declaration

```text
Task RemoveBoxGroup(RemoveBoxGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveBoxGroupArgs.html) | args | 要移除盒子分组的信息参数[RemoveBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveBoxGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveDataMonitorGroup\(RemoveDataMonitorGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveDataMonitorGroup_FBoxClientDriver_Contract_RemoveDataMonitorGroupArgs_"></a>

移除监控点组

#### Declaration

```text
Task RemoveDataMonitorGroup(RemoveDataMonitorGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveDataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveDataMonitorGroupArgs.html) | args | 移除监测点组别参数[RemoveDataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveDataMonitorGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveDataMonitorPoint\(RemoveDataMonitorDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveDataMonitorPoint_FBoxClientDriver_Contract_RemoveDataMonitorDefinitionArgs_"></a>

移除监控点条目

#### Declaration

```text
[Obsolete]
Task RemoveDataMonitorPoint(RemoveDataMonitorDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveDataMonitorDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveDataMonitorDefinitionArgs.html) | args | 移除监测点信息参数[RemoveDataMonitorDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveDataMonitorDefinitionArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveDataMonitorPointV2\(RemoveDataMonDefArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveDataMonitorPointV2_FBoxClientDriver_Contract_RemoveDataMonDefArgsV2_"></a>

删除监控点条目V2\(支持离线编辑\)

#### Declaration

```text
Task RemoveDataMonitorPointV2(RemoveDataMonDefArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveDataMonDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveDataMonDefArgsV2.html) | args | 删除监控点参数 |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 无 |

### RemoveHdataDefinitionV2\(RemoveHdataArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveHdataDefinitionV2_FBoxClientDriver_Contract_RemoveHdataArgsV2_"></a>

删除历史记录条目

#### Declaration

```text
[Obsolete]
Task RemoveHdataDefinitionV2(RemoveHdataArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveHdataArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveHdataArgsV2.html) | args | 删除历史记录参数[RemoveHdataArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveHdataArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### RemoveHdataItem\(RemoveHdataItemArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveHdataItem_FBoxClientDriver_Contract_RemoveHdataItemArgs_"></a>

移除历史记录多通道条目

#### Declaration

```text
Task RemoveHdataItem(RemoveHdataItemArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveHdataItemArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveHdataItemArgs.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### RemoveHistroyDefinition\(RemoveHistoryDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_RemoveHistroyDefinition_FBoxClientDriver_Contract_RemoveHistoryDefinitionArgs_"></a>

删除历史记录条目

#### Declaration

```text
[Obsolete]
Task RemoveHistroyDefinition(RemoveHistoryDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [RemoveHistoryDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.RemoveHistoryDefinitionArgs.html) | args | 删除历史监控点参数 [RemoveHistroyDefinition\(RemoveHistoryDefinitionArgs\)]() |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### Restart\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_Restart"></a>

实现切换用户登录初始化信息

#### Declaration

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### SetBoxDeviceConfigurationSource\(SetBoxDeviceConfigurationSourceArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_SetBoxDeviceConfigurationSource_FBoxClientDriver_Contract_SetBoxDeviceConfigurationSourceArgs_"></a>

#### Declaration

```text
Task SetBoxDeviceConfigurationSource(SetBoxDeviceConfigurationSourceArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [SetBoxDeviceConfigurationSourceArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.SetBoxDeviceConfigurationSourceArgs.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### Start\(\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_Start"></a>

启动

#### Declaration

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartAllDataMonitorPointsOnBox\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartAllDataMonitorPointsOnBox_FBoxClientDriver_Contract_BoxArgs_"></a>

开启指定盒子上所有监控点的数据推送

#### Declaration

```text
Task StartAllDataMonitorPointsOnBox(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子信息参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartDataMonitorGroup\(DataMonitorGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartDataMonitorGroup_FBoxClientDriver_Contract_DataMonitorGroupArgs_"></a>

开启某监控点组别数据推送

#### Declaration

```text
Task StartDataMonitorGroup(DataMonitorGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupArgs.html) | args | 开始监测点某组别数据推送参数[DataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartDataMonitorGroups\(DataMonitorGroupsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartDataMonitorGroups_FBoxClientDriver_Contract_DataMonitorGroupsArgs_"></a>

开启指定监控点组的数据推送

#### Declaration

```text
Task StartDataMonitorGroups(DataMonitorGroupsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupsArgs.html) | args | 开启指定监控点组的数据推送参数[DataMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartDataMonitorPoint\(DataMonitorPointArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartDataMonitorPoint_FBoxClientDriver_Contract_DataMonitorPointArgs_"></a>

开启监测点

#### Declaration

```text
Task StartDataMonitorPoint(DataMonitorPointArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointArgs.html) | args | 开启监测点参数[DataMonitorPointArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartDataMonitorPoints\(DataMonitorPointsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartDataMonitorPoints_FBoxClientDriver_Contract_DataMonitorPointsArgs_"></a>

开始某些检测点

#### Declaration

```text
Task StartDataMonitorPoints(DataMonitorPointsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) | args | 开始某些检测点参数[DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartDataMonitorPointsByGroupedName\(DataMonitorPointsByGroupedNameArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartDataMonitorPointsByGroupedName_FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs_"></a>

#### Declaration

```text
Task StartDataMonitorPointsByGroupedName(DataMonitorPointsByGroupedNameArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsByGroupedNameArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsByGroupedNameArgs.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### StartDmonItemsByNames\(StartDmonItemByNamesArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartDmonItemsByNames_FBoxClientDriver_Contract_StartDmonItemByNamesArgs_"></a>

根据名称开启监控

#### Declaration

```text
Task StartDmonItemsByNames(StartDmonItemByNamesArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [StartDmonItemByNamesArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StartDmonItemByNamesArgs.html) | args | 参数[StartDmonItemsByNames\(StartDmonItemByNamesArgs\)]() |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### StartSpecificDataMonitorPointsByGroupedNameOnly\(DataMonitorPointsByGroupedNameArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartSpecificDataMonitorPointsByGroupedNameOnly_FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs_"></a>

#### Declaration

```text
Task StartSpecificDataMonitorPointsByGroupedNameOnly(DataMonitorPointsByGroupedNameArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsByGroupedNameArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsByGroupedNameArgs.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### StartSpecificDataMonitorPointsByNameOnly\(DataMonitorPointsByNameArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartSpecificDataMonitorPointsByNameOnly_FBoxClientDriver_Contract_DataMonitorPointsByNameArgs_"></a>

开始某些检测点

#### Declaration

```text
Task StartSpecificDataMonitorPointsByNameOnly(DataMonitorPointsByNameArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsByNameArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsByNameArgs.html) | args | 开始某些检测点参数[DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartSpecifiedDataMonitorGroupOnly\(DataMonitorGroupsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartSpecifiedDataMonitorGroupOnly_FBoxClientDriver_Contract_DataMonitorGroupsArgs_"></a>

只开启指定的监测点组

#### Declaration

```text
Task StartSpecifiedDataMonitorGroupOnly(DataMonitorGroupsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupsArgs.html) | args | 监测点组别参数[DataMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StartSpecifiedDataMonitorPointsOnly\(DataMonitorPointsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StartSpecifiedDataMonitorPointsOnly_FBoxClientDriver_Contract_DataMonitorPointsArgs_"></a>

只开启指定的监测点

#### Declaration

```text
Task StartSpecifiedDataMonitorPointsOnly(DataMonitorPointsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) | args | 监测点参数[DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StopAllDataMonitorPointsOnBox\(BoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopAllDataMonitorPointsOnBox_FBoxClientDriver_Contract_BoxArgs_"></a>

停止指定盒子上所有监控点的数据推送

#### Declaration

```text
Task StopAllDataMonitorPointsOnBox(BoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) | args | 盒子信息参数[BoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StopDataMonitorGroup\(DataMonitorGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopDataMonitorGroup_FBoxClientDriver_Contract_DataMonitorGroupArgs_"></a>

停止某监控点组别数据推送

#### Declaration

```text
Task StopDataMonitorGroup(DataMonitorGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupArgs.html) | args | 停止某监控点组别数据推送参数[DataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StopDataMonitorGroups\(DataMonitorGroupsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopDataMonitorGroups_FBoxClientDriver_Contract_DataMonitorGroupsArgs_"></a>

停止指定监控点组的数据推送

#### Declaration

```text
Task StopDataMonitorGroups(DataMonitorGroupsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupsArgs.html) | args | 停止指定监控点组的数据推送[DataMonitorGroupsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorGroupsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StopDataMonitorPoint\(DataMonitorPointArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopDataMonitorPoint_FBoxClientDriver_Contract_DataMonitorPointArgs_"></a>

停止监测点

#### Declaration

```text
Task StopDataMonitorPoint(DataMonitorPointArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointArgs.html) | args | 停止监测点参数[DataMonitorPointArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StopDataMonitorPoints\(DataMonitorPointsArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopDataMonitorPoints_FBoxClientDriver_Contract_DataMonitorPointsArgs_"></a>

停止某些监测点

#### Declaration

```text
Task StopDataMonitorPoints(DataMonitorPointsArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) | args | 停止某些监测点参数[DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StopDataMonitorPointsByGroupedName\(DataMonitorPointsByGroupedNameArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopDataMonitorPointsByGroupedName_FBoxClientDriver_Contract_DataMonitorPointsByGroupedNameArgs_"></a>

#### Declaration

```text
Task StopDataMonitorPointsByGroupedName(DataMonitorPointsByGroupedNameArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsByGroupedNameArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsByGroupedNameArgs.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### StopDataMonitorPointsByName\(DataMonitorPointsByNameArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopDataMonitorPointsByName_FBoxClientDriver_Contract_DataMonitorPointsByNameArgs_"></a>

停止某些监测点

#### Declaration

```text
Task StopDataMonitorPointsByName(DataMonitorPointsByNameArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorPointsByNameArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsByNameArgs.html) | args | 停止某些监测点参数[DataMonitorPointsArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorPointsArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### StopDmonItemsByNames\(StopDmonItemByNamesArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_StopDmonItemsByNames_FBoxClientDriver_Contract_StopDmonItemByNamesArgs_"></a>

根据名称关闭监控点

#### Declaration

```text
Task StopDmonItemsByNames(StopDmonItemByNamesArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [StopDmonItemByNamesArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.StopDmonItemByNamesArgs.html) | args | 参数[StopDmonItemsByNames\(StopDmonItemByNamesArgs\)]() |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### UnregisterBox\(UnregisterBoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UnregisterBox_FBoxClientDriver_Contract_UnregisterBoxArgs_"></a>

删除注册盒子,不删除盒子内部数据

#### Declaration

```text
Task UnregisterBox(UnregisterBoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UnregisterBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UnregisterBoxArgs.html) | args | 要删除注册的盒子参数[UnregisterBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UnregisterBoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UnregisterBoxV2\(UnregisterBoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UnregisterBoxV2_FBoxClientDriver_Contract_UnregisterBoxArgs_"></a>

#### Declaration

```text
Task UnregisterBoxV2(UnregisterBoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UnregisterBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UnregisterBoxArgs.html) | args |  |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

### UpdateAlarmDefinition\(UpdateAlarmDefinitonArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateAlarmDefinition_FBoxClientDriver_Contract_UpdateAlarmDefinitonArgs_"></a>

更新报警条目

#### Declaration

```text
[Obsolete]
Task UpdateAlarmDefinition(UpdateAlarmDefinitonArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateAlarmDefinitonArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmDefinitonArgs.html) | args | 更细报警条目参数[UpdateAlarmDefinitonArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmDefinitonArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateAlarmDefinitionV2\(UpdateAlarmDefArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateAlarmDefinitionV2_FBoxClientDriver_Contract_UpdateAlarmDefArgsV2_"></a>

更新报警监控条目V2（支持离线编辑）

#### Declaration

```text
Task UpdateAlarmDefinitionV2(UpdateAlarmDefArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateAlarmDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmDefArgsV2.html) | args | 修改报警条目参数[UpdateAlarmDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmDefArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateAlarmGroup\(UpdateAlarmGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateAlarmGroup_FBoxClientDriver_Contract_UpdateAlarmGroupArgs_"></a>

更新报警分组

#### Declaration

```text
Task UpdateAlarmGroup(UpdateAlarmGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateAlarmGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmGroupArgs.html) | args | 跟新报警分组参数[UpdateAlarmGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateAlarmGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateAlarmTarget\(UpdateTargetArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateAlarmTarget_FBoxClientDriver_Contract_UpdateTargetArgs_"></a>

更新报警联系人

#### Declaration

```text
Task UpdateAlarmTarget(UpdateTargetArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateTargetArgs.html) | args | 更新报警联系人参数[UpdateTargetArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateTargetArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateBox\(UpdateBoxArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateBox_FBoxClientDriver_Contract_UpdateBoxArgs_"></a>

更新盒子

#### Declaration

```text
Task UpdateBox(UpdateBoxArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateBoxArgs.html) | args | 要更新的盒子参数[UpdateBoxArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateBoxArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateBoxGroup\(UpdateBoxGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateBoxGroup_FBoxClientDriver_Contract_UpdateBoxGroupArgs_"></a>

更新盒子分组

#### Declaration

```text
Task UpdateBoxGroup(UpdateBoxGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateBoxGroupArgs.html) | args | 要更新盒子分组的的参数信息 [UpdateBoxGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateBoxGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateDataMonitorGroup\(UpdateDataMonitorGroupArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateDataMonitorGroup_FBoxClientDriver_Contract_UpdateDataMonitorGroupArgs_"></a>

更新监控点组

#### Declaration

```text
Task UpdateDataMonitorGroup(UpdateDataMonitorGroupArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateDataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDataMonitorGroupArgs.html) | args | 更新监测点组别参数[UpdateDataMonitorGroupArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDataMonitorGroupArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateDataMonitorPoint\(UpdateDataMonitorDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateDataMonitorPoint_FBoxClientDriver_Contract_UpdateDataMonitorDefinitionArgs_"></a>

更新监控点条目

#### Declaration

```text
[Obsolete]
Task UpdateDataMonitorPoint(UpdateDataMonitorDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateDataMonitorDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDataMonitorDefinitionArgs.html) | args | 更新监测点信息参数[UpdateDataMonitorDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDataMonitorDefinitionArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateDataMonitorPointV2\(UpdateDmonArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateDataMonitorPointV2_FBoxClientDriver_Contract_UpdateDmonArgsV2_"></a>

更新监控点条目V2\(支持离线编辑\),集合长度不要超过20个

#### Declaration

```text
Task UpdateDataMonitorPointV2(UpdateDmonArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateDmonArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDmonArgsV2.html) | args | 更新监控点参数[UpdateDmonArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateDmonArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 无 |

### UpdateHdataDefinitionV2\(UpdateHdataDefArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateHdataDefinitionV2_FBoxClientDriver_Contract_UpdateHdataDefArgsV2_"></a>

更新历史记录条目

#### Declaration

```text
[Obsolete]
Task UpdateHdataDefinitionV2(UpdateHdataDefArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateHdataDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataDefArgsV2.html) | args | 更新历史记录条目参数[UpdateHdataDefArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataDefArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateHdataItems\(UpdateHdataItemArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateHdataItems_FBoxClientDriver_Contract_UpdateHdataItemArgs_"></a>

更新历史记录多通道

#### Declaration

```text
Task UpdateHdataItems(UpdateHdataItemArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateHdataItemArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataItemArgs.html) | args | 更新历史记录多通道参数[UpdateHdataItemArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHdataItemArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | System.Int64 |

### UpdateHistoryDefinition\(UpdateHDataDefinitionArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateHistoryDefinition_FBoxClientDriver_Contract_UpdateHDataDefinitionArgs_"></a>

更新历史记录条目

#### Declaration

```text
[Obsolete]
Task UpdateHistoryDefinition(UpdateHDataDefinitionArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateHDataDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHDataDefinitionArgs.html) | args | 更新历史监控点参数 [UpdateHDataDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateHDataDefinitionArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### UpdateRefreshTimeConfig\(UpdateRefreshTimeArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_UpdateRefreshTimeConfig_FBoxClientDriver_Contract_UpdateRefreshTimeArgs_"></a>

更新盒子数据条目刷新时间（盒子全局设置）

#### Declaration

```text
Task UpdateRefreshTimeConfig(UpdateRefreshTimeArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [UpdateRefreshTimeArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateRefreshTimeArgs.html) | args | 刷新盒子刷新时间[UpdateRefreshTimeArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.UpdateRefreshTimeArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### WriteValue\(DataMonitorWriteValueArgs\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_WriteValue_FBoxClientDriver_Contract_DataMonitorWriteValueArgs_"></a>

监控点写值

#### Declaration

```text
Task WriteValue(DataMonitorWriteValueArgs args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorWriteValueArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorWriteValueArgs.html) | args | 写入监测点值参数[DataMonitorWriteValueArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorWriteValueArgs.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task | 空 |

### WriteValue\(DataMonitorWriteValueArgsV2\) <a id="FBoxClientDriver_Contract_IFBoxClientManager_WriteValue_FBoxClientDriver_Contract_DataMonitorWriteValueArgsV2_"></a>

监控点写值V2,要求每个用户下监控点条目名称不一样

#### Declaration

```text
Task WriteValue(DataMonitorWriteValueArgsV2 args)
```

#### Parameters

| Type | Name | Description |
| :--- | :--- | :--- |
| [DataMonitorWriteValueArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorWriteValueArgsV2.html) | args | 写入监控点参数[DataMonitorWriteValueArgsV2](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorWriteValueArgsV2.html) |

#### Returns

| Type | Description |
| :--- | :--- |
| System.Threading.Tasks.Task |  |

## Events <a id="events"></a>

### AlarmConfirmed <a id="FBoxClientDriver_Contract_IFBoxClientManager_AlarmConfirmed"></a>

报警还原事件

#### Declaration

```text
event EventHandler> AlarmConfirmed
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;System.Collections.Generic.IList&lt;[AlarmConfirmDefinitonArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmConfirmDefinitonArgs.html)&gt;&gt; | 报警条目确认消息推送事件FBoxClientDriver.Contract.IFBoxClientManager.add\_AlarmConfirmed\(System.EventHandler{System.Collections.Generic.IList{FBoxClientDriver.Contract.AlarmConfirmDefinitonArgs}}\) |

### AlarmRecoverd <a id="FBoxClientDriver_Contract_IFBoxClientManager_AlarmRecoverd"></a>

报警还原事件

#### Declaration

```text
event EventHandler> AlarmRecoverd
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;System.Collections.Generic.IList&lt;[AlarmRecoverDefinitonArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmRecoverDefinitonArgs.html)&gt;&gt; |  |

### AlarmTriggered <a id="FBoxClientDriver_Contract_IFBoxClientManager_AlarmTriggered"></a>

报警触发事件

#### Declaration

```text
event EventHandler> AlarmTriggered
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;System.Collections.Generic.IList&lt;[AlarmTriggerDefinitionArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.AlarmTriggerDefinitionArgs.html)&gt;&gt; |  |

### BoxConnectStateChanged <a id="FBoxClientDriver_Contract_IFBoxClientManager_BoxConnectStateChanged"></a>

盒子状态变更事件

#### Declaration

```text
event EventHandler> BoxConnectStateChanged
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;System.Collections.Generic.IList&lt;[BoxConnectionStateItem](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.BoxConnectionStateItem.html)&gt;&gt; |  |

### BoxServerSignalRDisconnect <a id="FBoxClientDriver_Contract_IFBoxClientManager_BoxServerSignalRDisconnect"></a>

#### Declaration

```text
event EventHandler BoxServerSignalRDisconnect
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler |  |

### DataMonitorValueChanged <a id="FBoxClientDriver_Contract_IFBoxClientManager_DataMonitorValueChanged"></a>

监控点值数据变更事件

#### Declaration

```text
event EventHandler> DataMonitorValueChanged
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;System.Collections.Generic.IList&lt;[DataMonitorValueChangedArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DataMonitorValueChangedArgs.html)&gt;&gt; |  |

### MainServerSignalRDisconnect <a id="FBoxClientDriver_Contract_IFBoxClientManager_MainServerSignalRDisconnect"></a>

#### Declaration

```text
event EventHandler MainServerSignalRDisconnect
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;System.String&gt; |  |

### OnBoxLocationChanged <a id="FBoxClientDriver_Contract_IFBoxClientManager_OnBoxLocationChanged"></a>

盒子地理位置事件

#### Declaration

```text
event EventHandler OnBoxLocationChanged
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;[BoxLocationEventArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.SignalREventArgs.BoxLocationEventArgs.html)&gt; |  |

### OnBoxRegisterEvent <a id="FBoxClientDriver_Contract_IFBoxClientManager_OnBoxRegisterEvent"></a>

盒子注册通知事件

#### Declaration

```text
event EventHandler OnBoxRegisterEvent
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;[BoxRegisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxRegisterArgs.html)&gt; | 盒子注册触发事件，目前是广播的，可能收到别人注册的消息[BoxRegisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxRegisterArgs.html) |

### OnBoxUnregisterEvent <a id="FBoxClientDriver_Contract_IFBoxClientManager_OnBoxUnregisterEvent"></a>

盒子注销通知事件

#### Declaration

```text
event EventHandler OnBoxUnregisterEvent
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;[BoxUnRegisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxUnRegisterArgs.html)&gt; | 盒子注销触发事件，目前是广播，可能受到别人的注销信息[BoxUnRegisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.BoxUnRegisterArgs.html) |

### OnDMonRegisterEvent <a id="FBoxClientDriver_Contract_IFBoxClientManager_OnDMonRegisterEvent"></a>

盒子监控点注册事件

#### Declaration

```text
event EventHandler OnDMonRegisterEvent
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;[DMonRegisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonRegisterArgs.html)&gt; | 盒子监控点注册事件 [DMonRegisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonRegisterArgs.html) |

### OnDMonUnregisterEvent <a id="FBoxClientDriver_Contract_IFBoxClientManager_OnDMonUnregisterEvent"></a>

盒子监控删除事件

#### Declaration

```text
event EventHandler OnDMonUnregisterEvent
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;[DMonDefUnregisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonDefUnregisterArgs.html)&gt; | 盒子监控点删除事件 [DMonDefUnregisterArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.DMonDefUnregisterArgs.html) |

### OnSignalRMessageEvent <a id="FBoxClientDriver_Contract_IFBoxClientManager_OnSignalRMessageEvent"></a>

SignalR消息事件

#### Declaration

```text
event EventHandler OnSignalRMessageEvent
```

#### Event Type

| Type | Description |
| :--- | :--- |
| System.EventHandler&lt;[SignalRMessageArgs](https://docs.flexem.net/fbox/zh-cn/sdk/FBoxClientDriver.Contract.SignalRMessageArgs.html)&gt; |  |

