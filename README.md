## README

ant-design@4.23.6

### 构建

```shell
# node v18.16.0
yarn
npm run dist
```

### 配置

修改`node_modules\@ant-design\tools\lib\getWebpackConfig.js`文件

```shell
# 60行新增
babelConfig.sourceMap = true
# 62行修改
devtool: 'cheap-module-source-map'
```

`tsconfig.json`增加`sourcemap`配置

```shell
"sourceMap": true
```
