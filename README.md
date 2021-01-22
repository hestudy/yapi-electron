# Yapi Desktop

使用Electron构建Yapi桌面应用

- 已经自带cross-request插件，实现跨域

## 使用

更改app/main.js加载的地址即可

```javascript
// 改成你的内网部署地址
await mainWindow.loadURL("http://192.168.5.24:2333/")
```

## 运行

```shell script
npm run start
```

## 打包

### 首先全局安装electron-packager

```shell script
npm install -g electron-packager
```

### 然后执行打包

```shell script
electron-packager . Yapi --out=./dist --download.mirrorOptions.mirror=https://npm.taobao.org/mirrors/electron/
```
