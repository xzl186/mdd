# magma-front

> magma

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run all tests
npm test
```

## 技术站
| 类型 | 名称 |
| --- | --- |
| 开发语言|[node](https://nodejs.org/zh-cn/) |
| JS框架|[vue.js](https://github.com/vuejs/vue) |
| 模板引擎|[pug](https://github.com/pugjs/pug) |
| 构建工具|[webpack](https://github.com/webpack/webpack) |
| CSS预处理|[scss](http://sass-lang.com/) |
| 代码质量|[eslint](https://github.com/eslint/eslint) |
| UI框架 | [element](https://github.com/ElemeFE/element)  |
| 表格组件|[echarts](https://github.com/apache/incubator-echarts) |
| http客户端|[axios](https://github.com/axios/axios) |
| web认证|[jwt](https://jwt.io/introduction) |
| 字体图标|[font](http://fontawesome.dashgame.com) |
| mock数据|[mockJs](http://mockjs.com/) |


## mock
### mock 规则
  1. url添加`.mock`
  2. mock数据要放到`mock-server/mockdatas`目录下，
  3. mock文件命名格式与接口名对应，如：后台借口为`/v1/menu`，那么mock的数据文件名为`V1Menu.json`
  4. mock 使用仅限开发过程中使用，代码提交前要剔除`.mock` 接口
For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

## 开发指南
### welcome page
1. 需求页面
   开发登录后默认页面
   页面内容包含已有后台系统快捷方式
   * 视频配置后台系统 http://video.admin.intra.weibo.com:29090/
   * 视频综合后台系统 10.77.6.162:8080
   * muses http://10.75.0.24:10135/muses/
2. 创建页面
    * 在`/src/pages`目录下创建文件夹和文件`welcome/index.vue`
    * 复制demo下的HelloWrold.vue 中的代码到新创建的vue页面中，
    * 根据业务情况替换页面中的内容  
        ![](http://ww1.sinaimg.cn/large/7c04b661ly1frfixpo8oqj20mm0hkdip.jpg)
    * 在style 区域内便也页面样式（可以提取文件sass再倒入到此区域`@import`）
    * 在script区域内便也网页脚本（可以提取额文件js再倒入到此区域`import`）

3. 路由配置
  * 在`/src/router/index.js` 添加路由配置
    * 导入vue模块 `import Welcome from '../pages/welcome/index'`
    * 配置请求路由
    
         `{
                path: 'welcome', //路由请求地址
                name: 'welcome',
                component: Welcome
          },`
4. 将路由配置到菜单中（在左侧显示）
5. 









