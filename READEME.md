## 使用VitePress搭建及部署vue组件库文档

### 安装vitepress

```js
 pnpm add vitepress vue -D
 ```
在 package.json添加一些script

```js
 "scripts": {
    "docs:dev": "vitepress dev docs",
    "docs:build": "vitepress build docs",
    "docs:serve": "vitepress serve docs",
    "deploy": "deploy.sh",
  }
```

### deploy 部署

  - 手动部署
    > 新建 deploy.sh文件，配置部署信息，运行：npm run deploy

  - 自动部署
    > 新建 .github/workflows/deploy.yml 文件，配置部署信息，每次 git push后，自动打包部署到GitHub的gh-pages分支上

