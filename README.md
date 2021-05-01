### 项目整体文件说明
- `config` 配置文件目录
  - `default.json` 默认配置文件（其中包含数据库配置，jwt配置）
- `dao` 数据访问层，存放对数据库的增删改查操作
  - `DAO.js` 提供的公共访问数据库的方法
- `db`
  - mydb.sql 数据库文件
- `models` 存放具体数据库 ORM 模型文件
- `modules` 当前项目模块
  - `authorization.js` API权限验证模块
  - `database.js` 数据库模块（数据库加载基于 nodejs-orm2 库加载）
  - `passport.js` 基于 passport 模块的登录搭建
  - `resextra.js` API 统一返回结果接口
- `node_modules` 项目依赖的第三方模块
- `routes` 统一路由
  - `api` 提供 api 接口
  - `mapp` 提供移动APP界面
  - `mweb` 提供移动web站点
- `services` 服务层，业务逻辑代码在这一层编写，通过不同的接口获取的数据转换成统一的前端所需要的数据
- `app.js` 主项目入口文件
- `package.json` 项目配置文件

### 项目环境

##### 	本地环境

​		Node.js + MySQL

##### 	创建数据库

- 数据库文件在：db -> mysdb.sql
  - 创建数据库mydb，可通过新建查询执行mysdb.sql下的SQL语句建立数据库，数据库表
- 数据库连接名：root    密码： 123456
  - 可在config -> default.json 修改


##### 	启动项目

- 方法一：（推荐）
  - 已进行批处理，直接点击 start.bat 即可启动项目
- 方法二：
  - 安装依赖： npm install
  - 启动项目 ：node app.js

### 注：
**在项目[vue_mall_manager](https://github.com/chloeeee72/vue-mall-manager)中，需要连接数据库**
**方法：**
**1、按照方法一启动该项目**
**2、在navicat中创建连接 -> 新建数据库 -> 启动 mydb.sql 文件**
**3、按照[vue_mall_manager](https://github.com/chloeeee72/vue-mall-manager)中README.MD文件启动vue项目**
