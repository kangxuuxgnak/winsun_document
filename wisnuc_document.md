# wisnuc打包命令

## 安装git：sudo apt install git
！[安裝git]（./1.png)


## 克隆代码：git clone https://www.github.com/wisnuc/fruitmix-desktop.git
！[克隆代码]（./2.png)


## 切换到代码目录查看：cd fruitmix-desktop
！[切换目录]（./3.png)


## 切换分支：git checkout transimission
！[切换分支]（./4.png)


## 安装依赖包：  npm install （全局情况下安装依赖包：  npm install –g）
！[安装依赖包]（./5.png)


## 前端进行打包：   node_modules/.bin/webpack --watch --watch-poll
##（全局情况下前端进行打包：webpack）
！[前端进行打包]（./6.png)


## Fruitmix-desktop去杂，缩减储存占用
！[去杂]（./7.png)



## 将es6语法编译为浏览器支持的es5： npm run build
！[降维]（./8.png)


## 去除node_modules杂余文件：   npm prune –production
！[去杂]（./9.png)


## 查询打包基础命令： node_modules/.bin/electron-packager –help
##（全局时查询命令：          electron-packager –help）
## 找到arch和platform的对应值。
！[查询]（./10.png)


## linux打包：     node_modules/.bin/electron-packager . --no-prune --arch=x64 --platform=linux
##（全局时打包命令：          electron-packager . --no-prune --arch=x64 --platform=linux）
！[linux]（./11.png)


## windows打包：

#（1）.安装windows依赖包：
# sudo apt install wine

# sudo dpkg --configure –a

# sudo apt install wine
！[windows依赖包]（./12.png)

#（2）.windows64位进行打包： node_modules/.bin/electron-packager . --no-prune --arch=x64 --platform=win32

# Windows32位进行打包：  node_modules/.bin/electron-packager . --no-prune --arch=ia32 --platform=win32

# （全局时打包命令：          electron-packager . --no-prune --arch=x64 --platform=win32）
！[windows]（./13.png)


## mac打包：  node_modules/.bin/electron-packager . --no-prune --arch=x64 --platform= darwin
## （全局时mac打包命令：          electron-packager . --no-prune --arch=x64 --platform=darwin）


## 查看成功与否
！[查看成功与否]（./15.png)


完毕。



















