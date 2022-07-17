# zz-ui

[zz-ui]()

## 使用 monorepo

> 使用 yarn workspace

#### 给指定 package 安装包
```
yarn workspace zz-button add echarts
```

## 使用 storybook

> 使用 yarn 安装依赖

1. npx sb init --type vue3
2. yarn add vue
3. yarn add vue-loader vue-template-compiler -D -W

## 单元测试

- Vue Test Utils
- Jest
- Vue Jest
- Babel Jest

```
yarn add jest @vue/test-utils vue-jest@5 babel-jest -D -W

yarn add babel-core@bridge -D -W
```

## 使用 rollup 打包

### 打包单个组件

```
yarn add rollup rollup-plugin-terser rollup-plugin-vue vue-template-compiler -D -W
```

### 打包所有组件

```
yarn add @rollup/plugin-json rollup-plugin-postcss @rollup/plugin-node-resolve -D -W
```

## 环境变量

```
yarn add cross-env -D -W
```

## 清理目录

```
yarn add rimraf -D -W
```

## 生成组件模板

```
yarn add plop -D -W
```
