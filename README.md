
-	Team work. Build a website that realize a Kanban application and deploy it to a cloud server. 
-	My contribution (Wang Mingye's contribution): As the group leader, arrange the work in each iteration and assign tasks to team members reasonably. Besides, I was responsible for developing backend API of the site and deploying the project.




# Final-Work
> 一款项目管理软件：Ultimate Project – The Ultimate Tool for PM

- [Final-Work](#final-work)
  - [目录结构说明](#目录结构说明)
    - [1. docs目录](#1-docs目录)
    - [2. codes目录](#2-codes目录)
  - [课件08的团队作业安排（写于2020.07.30）](#课件08的团队作业安排写于20200730)
    - [0. **\*务必阅读\*** 整体要求](#0-务必阅读-整体要求)
    - [1. 以软件质量模型为依据，收集系统“非功能”需求与场景](#1-以软件质量模型为依据收集系统非功能需求与场景)
    - [3. 软件测试](#3-软件测试)
      - [I. 静态代码分析](#i-静态代码分析)
      - [II. 单元与集成测试、测试用例](#ii-单元与集成测试测试用例)
      - [III. CI/CD流水线构建与部署：](#iii-cicd流水线构建与部署)
  - [课件07的团队作业安排（写于2020.07.23）](#课件07的团队作业安排写于20200723)
    - [0. **\*务必阅读\*** 整体要求、阶段总结与DDL](#0-务必阅读-整体要求阶段总结与ddl)
    - [1. 故事板](#1-故事板)
    - [2. 迭代计划](#2-迭代计划)
    - [3. 功能开发 代码+文档](#3-功能开发-代码文档)
    - [4. 总结与ppt](#4-总结与ppt)
  - [课件05的团队作业安排（写于2020.06.16）](#课件05的团队作业安排写于20200616)
    - [0. DDL](#0-ddl)
    - [1. 项目章程](#1-项目章程)
    - [2. 项目管理计划](#2-项目管理计划)
    - [3. 调查初步需求](#3-调查初步需求)
    - [4. “收集需求”的方法、过程与涉及的技术与工具 文档和PPT](#4-收集需求的方法过程与涉及的技术与工具-文档和ppt)





## 目录结构说明
### 1. docs目录
所有项目文档均储存在此目录.

对于任意一个markown文档A（即文件名后缀是.md的文件），其图片的储存目录应当放在该文档同目录下，并明命名为 `A_image`。 例如 `docs/test.md` 的图片储存目录应当是 `docs/test_image`。\

历次会议纪要：[docs/Project_Fundamental/meeting_summary.md](./docs/Project_Fundamental/meeting_summary.md)

### 2. codes目录
所有代码工程会保存在此目录。


## 课件08的团队作业安排（写于2020.07.30）

### 0. **\*务必阅读\*** 整体要求
记得使用看板。记得填写工作量文档[all_time_work_division.md](./all_time_work_division.md)

### 1. 以软件质量模型为依据，收集系统“非功能”需求与场景
软件质量模型：
- [https://blog.51cto.com/9797337/2398173](https://blog.51cto.com/9797337/2398173)
- [https://www.cnblogs.com/gaochundong/p/software_quality_models.html#quality_model_iso9126](https://www.cnblogs.com/gaochundong/p/software_quality_models.html#quality_model_iso9126)

收集系统“非功能”需求与场景的文档是 `docs/Project_Fundamental/non_func_requirements.md`

收集系统“非功能”需求与场景：黄冠纶、张弛、幸赟、陈剑锋

### 3. 软件测试
#### I. 静态代码分析
后端Python代码静态分析：使用Python静态代码分析工具 `flake8` （[使用教程https://www.cnblogs.com/Zzbj/p/11204411.html](https://www.cnblogs.com/Zzbj/p/11204411.html)）分析代码文件即可，将输出整理并记录到文档。后端Python代码在[codes/Backend](./codes/Backend)文件夹中。

后端Python代码静态分析：王嘉浚

前端Javascript代码静态分析：选用Javascript静态代码分析工具分析代码文件即可，将输出整理并记录到文档。

前端Javascript代码静态分析：王思博

静态代码分析的文档是 `docs/Quality/code_static_analysis.md`

#### II. 单元与集成测试、测试用例

后端Python代码：王明业

后端Python代码单元与集成测试、测试用例文档是 `docs/Quality/py_unit_and_integration_testing.md`

前端Javascript代码：张佳蔚，温卓沛

前端Javascript代码单元与集成测试、测试用例文档是 `docs/Quality/js_unit_and_integration_testing.md`




#### III. CI/CD流水线构建与部署：

参考：Github的Actions标签页可构建并部署CI流水线

CI/CD流水线：王子豪，顾子杉，吴明章，王子雄

CI/CD流水线构建与部署文档是：`docs/Quality/CI_CD_deployment.md`



## 课件07的团队作业安排（写于2020.07.23）

小组有可能把所有push任务交由组内一成员完成。所以用GitHub的push记录来判断绩效可能不准确，应当参考本作业安排。

### 0. **\*务必阅读\*** 整体要求、阶段总结与DDL

每个成员都要在本github仓库的看板中填写并管理自己的工作任务。本次作业看板：本代码仓库-`projects`标签页-[迭代管理（0805结束）](https://github.com/Invincible-Inc/Final-Work/projects/3)看板

**07.29晚上20:30** 召开阶段Sprint会议。

**08.03晚上20:30** 召开Sprint回顾会议。本次作业所有任务需要在08.03前完成。08.04一天时间整理与修改。

### 1. 故事板
Scrum and XP 书本第4页“我们怎样编写产品 backlog”。故事Story即Backlog。参考书上示例为我们的项目构建故事板（即Backlog表）。

故事板中的内容可参考上次作业中思博和明章总结的需求文档[https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements)

**注意：** 故事板中必须要有“[看板](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements#%E5%8A%9F%E8%83%BD3%E7%9C%8B%E6%9D%BF)”功能的条目。

本项目的故事板文档是 `docs/Project_Fundamental/backlog.md`，博客页面链接：[https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/backlog](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/backlog)

故事板：王思博、吴明章、黄冠纶

### 2. 迭代计划
迭代计划文档是 `docs/Project_Fundamental/iteration_plan.md`，博客页面链接：[https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/iteration_plan](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/iteration_plan)

迭代计划的时间跨度可以很长，内容可以很多。

迭代的需求目标同样可参考上次作业中思博和明章总结的需求文档[https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements)

**注意：** 迭代计划必须包含这次作业期间的任务，即“[看板](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements#%E5%8A%9F%E8%83%BD3%E7%9C%8B%E6%9D%BF)”的实现。

迭代计划：陈剑锋、顾子杉

### 3. 功能开发 代码+文档

开发看板功能

功能开发：王子豪、张佳蔚、温卓沛、王嘉浚、王明业

### 4. 总结与ppt

在本次作业后期安排

总结与ppt：王子雄、幸赟、张弛

## 课件05的团队作业安排（写于2020.06.16）

### 0. DDL
请大家在**06.23**中午12:00前完成并push到仓库，留一天时间整合、检查。

### 1. 项目章程
已完成。博客页面链接：[https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/project_charter](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/project_charter)

### 2. 项目管理计划
项目管理计划是 `docs/Project_Fundamental/project_management_plan.md`，博客页面链接：[https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/project_management_plan](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/project_management_plan) 其中有六个部分，可以根据提示完成，言之有理、叙述完整清楚即可。

- 变更管理计划：张佳蔚

- 配置管理计划：张弛

- 绩效测量基准：黄冠纶

- 项目生命周期：陈剑锋

- 开发方法：王子豪

- 管理审查：王子雄

### 3. 调查初步需求
需求文档是 `docs/Project_Fundamental/requirements.md`，博客页面链接：[https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements](https://invincible-inc.github.io/Final-Work/docs/Project_Fundamental/requirements)。可以根据提示完成。

调查初步需求：王思博、吴明章

### 4. “收集需求”的方法、过程与涉及的技术与工具 文档和PPT

文档是 `docs/Practice_and_Research/requirements_gathering_methods.md`，博客页面链接：[https://invincible-inc.github.io/Final-Work/docs/Practice_and_Research/requirements_gathering_methods](https://invincible-inc.github.io/Final-Work/docs/Practice_and_Research/requirements_gathering_methods)。可以根据提示完成。

PPT腾讯文档链接：[https://docs.qq.com/slide/DYm11dW1vS21iRG9j](https://docs.qq.com/slide/DYm11dW1vS21iRG9j)。

“收集需求”的方法 文档和PPT：温卓沛、幸赟、王嘉浚、顾子杉

