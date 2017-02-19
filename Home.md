# CloudTest看板

## 宗旨： 主动 负责 认真 大胆 务实 开创

[迭代看板](20.30.00.Current Sprint) | [产品Backlog] [2] | [Sprint Backlog] [3] | [版本信息] [4]

-----------------------------------------------

# CloudTest计划

## 总体

因为项目要求时间紧任务重，所以，在第一阶段之前略过自动化过程管理，质量过程等部分。

第一阶段直奔主题：解决问题，自行运维。

在第二阶段时考虑交付形式，交付内容，交付质量，自动化运维（devops）等方面的内容。

如果需要查看详细的项目计划可以：[项目计划] [1]

------------------------------------------------------

代码管理:

|模块|介绍|路径|代码量|分支|
|---|---|---|---|---|
|CloudTest|CloudTest的公共逻辑都在于此|http://github.xa.com/ct/CloudTest.git|26362|master|
|CloudTest.wiki|CloudTest项目文档|http://github.xa.com/ct/CloudTest.wiki.git||master|
|web|用于展示系统信息|http://github.xa.com/ct/web.git|61767|master|
|auth|分布式认证系统，自行开发未使用开源协议与代码|http://github.xa.com/ct/auth.git|1032|master|
|Master|最主要的处理都在于此。|http://github.xa.com/ct/Master.git|3889|master|
|Master-TaskManager|真实任务模拟任务的管理|http://github.xa.com/ct/Master-TaskManager.git|20564|master|
|Master-Resource|真实资源模拟资源的资源管理服务|http://github.xa.com/ct/Master-Resource.git|4701|master|
|Master-Gateway|API Gateway用来转发消息|http://github.xa.com/ct/Master-Gateway.git|3043|master|
|Master-ChartManager|用来生成流量图的地方|http://github.xa.com/ct/Master-ChartManager.git|2190|master|
|slave|真正控制代码执行的地方|http://github.xa.com/ct/slave.git|3086|master|
|Slave_UE|管理UE的点|http://github.xa.com/ct/Slave_UE.git|1262|master|
|testframework|测试框架|http://github.xa.com/ct/testframework.git|7313|master|
|Real-UE|安卓代码|http://github.xa.com/ct/Real-UE.git|29061|master|
|Sim-UE|超级不稳定的openair4g模拟UE代码|http://github.xa.com/ct/Sim-UE.git|1359581|master|
|CGI|真实环境中操作配置参数的CGI|http://github.xa.com/ct/CGI.git|349016|master|
|Microservice-Config||http://github.xa.com/ct/Microservice-Config.git||master|

共计：16个组建或模块，代码量300K。

------------------------------------------------------------------------------

## 第一阶段细化

**大任务优先级划分：**

|编号|故事|内容|工作量|优先级|重要度|
|---|---|---|---|---|---|
|1|现有平台稳定|满足95%的稳定性要求|30人日|95|95|
|2|平台展示优化|最大程度的提高用户体验|20人日|80|99|
|3|MESH两节点真实环境CI|开发MESH两节点，真实环境CI|30人日|93|99|
|4|LTE小站真实环境CI|开发LTE小站真实环境CI|30人日|92|99|
|5|系统手动运维与部署|现有环境的维护|10人日|93|99|
|6|新环境接入|新环境的接入MESH环境，LTE小站环境|10人日|92|99|

------------------------------------------

**风险控制：**

|编号|风险级别|风险|内容|应对措施|
|---|---|---|---|---|
|1|B|物料|1.小站物料问题<p>2.mesh的物料问题|1.尽量让物料问题不影响开发进度。<p>2.时刻跟进物料问题|
|2|A|终端代码维护|1.终端代码维护<p>2.终端代码所能适应的安卓版本问题<p>3.小站终端物料<p>4.小站终端的安卓代码的开发<p>5.终端代码的稳定性问题|1.组织学习终端代码<p>2.带着问题完成安卓开发的学习<p>|

-------------------------------------------

## 过程方法：


1. 任何事必须满足SMART原则，都必须是**明确的，可衡量的，可实现的，相关的，有时限的**。
- 使用Scurm方法来完成过程管理，以提高我们的执行力。
- 使用快速反馈方法来提高进度跟踪能力。


[1]: 20.10.项目计划 "项目计划"
[2]: 20.00.需求管理 "产品Backlog"
[3]: 20.10.项目计划 "Sprint Backlog"
[4]: 10.版本信息
