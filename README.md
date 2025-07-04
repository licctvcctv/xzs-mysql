# 在线考试系统

基于学之思开源考试系统修改的在线考试平台，已移除所有营销内容。

## 🚀 GitHub Actions 自动构建

本项目配置了GitHub Actions自动构建前端，方便开发和部署。

### 构建触发条件：
- 推送代码到 `main`、`master`、`dev` 分支
- 修改 `source/vue/` 目录下的文件
- 手动触发（在Actions页面点击"Run workflow"）

### 构建产物：
- `student-frontend-dist`: 学生端前端构建文件
- `admin-frontend-dist`: 管理端前端构建文件

### 使用方法：
1. 修改Vue源码后推送到GitHub
2. 等待Actions自动构建完成（约5-10分钟）
3. 在Actions页面下载构建产物
4. 将构建文件复制到Spring Boot的static目录

## 项目介绍

这是一款 Java + Vue 的前后端分离的考试系统。主要优点是开发、部署简单快捷、界面设计友好、代码结构清晰。支持web端和微信小程序，能覆盖到pc机和手机等设备。
支持多种部署方式：集成部署、前后端分离部署、docker部署。

## 技术栈

### 后端技术
- Spring Boot 2.1.6
- MyBatis
- MySQL 8.0
- Redis
- JWT

### 前端技术
- Vue.js 2.x
- Element UI
- Axios
- Vue Router



### 学生系统功能

|  模块   | 介绍  |
|  ----  | ----  |
| 登录  | 用户名、密码  |
| 注册  | 年级、用户名、密码  |
| 任务中心  | 管理员发布的年级任务，每个学生只能做一次  |
| 考试  | 题干支持文本、图片、数学公式、表格等，学生答题支持：文本  |
| 固定试卷  | 可重复练习、自行批改的试卷  |
| 时段试卷  | 在时间限制内，可重复练习、自行批改的试卷  |
| 考试记录  | 查看答卷记录和试卷信息  |
| 错题本  | 答错题目会自动进入错题本，显示题目基本信息  |
| 个人信息  | 显示学生个人资料  |
| 更新信息  | 修改个人资料、头像  |
| 个人动态  | 显示用户最近的个人动态  |
| 消息中心  | 用于接收管理员发送的消息  |

### 管理系统功能

|  模块   | 介绍  |
|  ----  | ----  |
| 登录  | 用户名、密码  |
| 主页  | 试卷总数、题目总数、用户活跃度、题目月数量  |
| 学生列表  | 显示系统所有的学生，新增、修改、删除、禁用  |
| 管理员列表  | 显示系统所有的管理员，新增、修改、删除、禁用  |
| 学科列表  | 学科查询、修改、删除  |
| 学科创编  | 创建学科  |
| 试卷列表  | 试卷查询、修改、删除  |
| 试卷创编  | 创建的试卷为时段试卷、固定试卷、任务试卷  |
| 题目列表  | 题目查询、修改、删除  |
| 题目创建  | 题目支持单选题、多选题、判断题、填空题、简答题，题干支持文本、图片、表格、数学公式  |
| 任务列表  | 任务查询、修改、删除  |
| 消息列表  | 显示已发送的消息，消息已读人数等信息  |
| 消息发送  | 发送消息给多个用户  |
| 用户日志  | 显示所有用户日志  |
| 个人资料  | 显示管理员用户名、真实姓名  |
| 时间线  | 显示管理员创建时间  |
| 修改资料  | 修改姓名、手机号  |

### 小程序功能

|  模块   | 介绍  |
|  ----  | ----  |
| 登录  | 用户登录登出功能，登录会自动绑定微信账号，登出会解绑  |
| 注册  | 年级、用户名、密码  |
| 任务中心  | 管理员发布的年级任务，每个学生只能做一次  |
| 考试  | 题干支持文本、图片、数学公式、表格等，学生答题支持：文本  |
| 固定试卷  | 可重复练习、自行批改的试卷  |
| 时段试卷  | 在时间限制内，可重复练习、自行批改的试卷  |
| 考试记录  | 查看答卷记录和试卷信息  |
| 错题本  | 答错题目会自动进入错题本，显示题目基本信息  |
| 个人信息  | 显示学生个人资料  |
| 更新信息  | 修改个人资料、头像  |
| 个人动态  | 显示用户最近的个人动态  |
| 消息中心  | 用于接收管理员发送的消息  |

### 系统展示

* 学生考试系统
<table>
    <tr>
        <td><img src="https://www.mindskip.net/style/git/images/student/1.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/student/2.png"/></td>
    </tr>
</table>

*  小程序考试系统
<table>
    <tr>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/1.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/2.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/3.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/4.png"/></td>
    </tr>
    <tr>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/10.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/8.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/6.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/wx/student/7.png"/></td>
    </tr>
</table>

* 后台管理系统

<table>
    <tr>
        <td><img src="https://www.mindskip.net/style/git/images/admin/1.png"/></td>
        <td><img src="https://www.mindskip.net/style/git/images/admin/2.png"/></td>
    </tr>
</table>