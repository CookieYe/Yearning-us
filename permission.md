# 权限设置

## 理念

**Yearning采用基于用户的细粒度权限/角色权限,权限最低下放至数据源。** 

**Yearning中用户先以角色的形式分为三大类,分别为 使用者/管理员/执行人。其中管理员/执行人角色为可见管理页面角色, 使用者为非可见管理页面角色。通过角色Yearning在细粒度权限划分之前先将用户分类。使管理类权限不会出现在使用者细粒度权限划分中** 

**可根据每个用户的实际需求配置相应ddl/dml/查询数据源。每一类权限相互独立互不干扰。**

**基于用户的拼图式权限可最大化保证细粒度权限的多样化,可实现对每一个用户都设置不同权限的目的。**

## 注意事项

首次使用Yearning时超级管理员本身也不具备对应的细粒度权限,需自行配置。 新建用户同样不具备任何权限。任何操作都必须在赋予对应的权限之后才能执行。所以**请在使用之前赋予用户权限**！


## 设置用户权限

### 基于用户自主申请

在Yearning中用户可通过**首页个人信息栏-查看权限按钮** 查看当前权限并可通过**申请权限按钮**提交权限申请。

该权限申请将会以工单的形式发送给超级管理员进行审批。(超级管理员为admin用户)如开启消息推送,该工单将会进行相应推送。

当超级管理员收到申请之后,可对相应权限工单进行**审阅/修改**。由于用户申请的权限可能并非实际应授予的权限。所以超级管理员可对权限工单进行直接修改,新增/删除相应权限。修改确认无误后点击同意，该用户权限将自动更新。

**注意**

为了防止用户过度提交权限申请。Yearning强制规定用户只有在之前的权限申请通过/驳回之后才能提交新的权限申请。

权限工单为**覆盖更新**并非增量更新,用户提交时因把**之前的权限与申请的权限**一起提交

同时超级管理员也可在**设置页面**设置每个用户单日最大权限申请数。 设置后每个用户一天之内申请权限次数不得超过设置的阈值

### 超级管理员直接修改

在Yearning中超级管理员可自行对任意用户的权限进行修改,如需修改 请前往用户权限页面进行相应设置。

