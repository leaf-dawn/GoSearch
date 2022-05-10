# Gopher搜搜way


### 目录结构
```basic

├─conf              存放配置文件
├─controllers       对外暴露接口的控制层
├─dictionary        字典数据
├─model             模型
├─routers           路由
├─searcher          核心功能架构包
│  ├─dump           备份文件
│  ├─model          模型
│  └─pagination     分页组件
├─srevice           基本业务处理类
└─util              工具类

```
### 提交规范
- 在github上建立自己的仓库并使用git进行版本管理
- Git 提交规范 `<type>(<scope>):<subject>`
- type 包括
  - feat：新功能（feature）
  - fix：修补bug
  - docs：文档（documentation）
  - style： 格式（不影响代码运行的变动）
  - refactor：重构（即不是新增功能，也不是修改bug的代码变动）
- scope 指影响范围，具体到包即可
- subject 指具体修改内容
  - 举例：feat(service) :添加账户注册功能
- 建立保护分支，不允许直接往主干分支上推送内容。如果需要更新主干分支内容，需要提出pull request 合并请求，在校验代码无误后合并
- Git 提交的粒度要足够小（原则上每次 commit 不超过 200 行，要求在 Pull Request 中看到的每个 commit 都是细粒度的），比如每完成一个功能或修复一个 bug 尽量都进行提交
