## 创建项目和初始化
1. npx create-react-app z-chat-web
2. npm install react-app-rewired customize-cra --dev<br>
[react-app-rewired](https://github.com/timarney/react-app-rewired)是react社区开源的一个修改CRA配置的工具，例如扩展Create React App的webpack配置，而[customize-cra](https://github.com/arackaf/customize-cra)提供了一组自定义利用react-app-rewired核心功能的Create React App v2配置，可以通过config-override.js文件来对webpack配置进行扩展<br>
## 多页应用配置
1. 修改入口文件<br>
1)&nbsp;删除默认入口文件src/index.js和相关依赖<br>
2)&nbsp;创建src/pages/index.js和src/pages/login.js<br>
3)&nbsp;编写两个入口文件<br>
4)&nbsp;多页应用应使用hashHistory
2. 自定义create-react-app配置