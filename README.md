# get

[![GPL-3.0](https://img.shields.io/badge/license-GPL--3.0-blue.svg)](LICENSE)

https://www.mtdhb.com 红包核心领取逻辑，需配合 [mtdhb/api](https://github.com/mtdhb/api) 使用

基于 [mtdhb/old](https://github.com/mtdhb/old) 改造，代码比较乱，自行研究和部署吧

## 环境

Node.js 9.x

### 开发

```bash
npm i
npm run dev
```

### 生产

#### 配置代理服务器

请修改 [src/service/proxy-server.js](src/service/proxy-server.js)

如果只有一个代理，也可以配置服务器环境变量

```bash
export PROXY_HOST=ip
export PROXY_PORT=port
```

#### 首次部署

```bash
npm i pm2 -g
npm i
npm start
```

#### 代码更新

```bash
npm run reload
```
