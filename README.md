## 说明

    一个试题生成器

## 功能模块
```


```

## 开发 & 运行
```
# 初始化项目

    git clone https://github.com/freewu/tests-generator.git
    cd tests-generator
    npm install

# 预览

    npm start

# 打包 

    npm run package
    
```

## 组件

<a target="_blank" href="https://github.com/electron-react-boilerplate/electron-react-boilerplate">Electron React Boilerplate</a>   
<a target="_blank" href="https://react.dev/">React 18</a>   
<a target="_blank" href="https://www.electronjs.org/">Electron 23</a>  
<a target="_blank" href="https://ant.design/">Ant Design 5</a>  


## 应用截图

## Q&A
```
## windows 打包出现下载 winCodeSign / nsis / nsis-resources 出错

    问题:
    Get "https://github.com/electron-userland/electron-builder-binaries/releases/download/nsis-resources-3.4.1/nsis-resources-3.4.1.7z": read tcp xxx.xxx.xxx.xxx:zzz->xxx.xxx.xxx.xxx:443: wsarecv: An existing connection was forcibly closed by the remote host.
    
    解决：
        1 复制链接，手动下载下来
        2 进入目录  C:\Users\<username>\AppData\Local\electron-builder\cache\
        3 把下载的文件解压（整体目录 ）
            winCodeSign-xx.7z 解压到 winCodeSign/winCodeSign-xx
            nsis-xx.7z 解压到 nsis/nsis-xx
            nsis-resources-xx.7z 解压到 nsis/nsis-resources-xx
        4 重新执行打包命令 npn run package

```

## 版本修改 (发布前需要修改)
```
./package.json  
./release/app/package.json
```