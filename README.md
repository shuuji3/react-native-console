# React Native Console v1.1.7
An IDEA/WebStorm/Android Studio Plugin for One-Click run React Native command, the No.1 WebStorm plugin for React Native developers

## Installation
First, please setup your React Native dev env:
https://facebook.github.io/react-native/docs/getting-started.html

Second, you can install it through your IDE, bring up  Preferences > Plugins > Browse repositories... , search for '**React Native Console**',
then you can install this plugin there.<br/>

Or<br/>you can munally install jar file react-native-console.jar as a plugin to your IDE. And the plugin home page is here: https://plugins.jetbrains.com/plugin/9564-react-native-console<br/><br/>

Now restart IDEA and enjoy!


## Note
Java 8 required to run the IDE.<br/>

## Settings(Optional, only need if js project dir can't be auto find)
Specify js project work directory rather than root directory, eg ./jsapp , now can from welcome screen or toolbar to edit this property. And the final value is stored in a file named .idea/.rnconsole, which content should like this:

```json
{
  currentPath: './jsapp'
}
```

after that all npm commands will use this as the working dir.

## Linux Users PLEASE README FIRST

If you found issue when click on the "Debug Android" button, error message: 
 "SDK location not found ", please fix it like this :
add a android local config file:
yourapp/android/local.properties
`sdk.dir=/Users/xxxx/Documents/Java/android-sdk-macosx`
let sdk.dir point to your ANDROID_HOME environment 
if can't find adb, try this shell command:

```sh
sudo ln -s ~/Android/Sdk/platform-tools/adb /usr/bin/adb
```


More info please ref this issue:
https://github.com/beansoftapp/react-native-console/issues/17


## Features
list and run scripts in package.json<br>One-Click run following commands:<br/>

run React Native Debugger https://github.com/jhen0409/react-native-debugger(Mac Only)

Ctrl + F2 to reload android js bundle<br>list and run scripts in package.json<br>react-native run-android<br/>react-native link<br/>react-native run-ios<br/>run with physical iOS device<br/>list all iOS devices(include simulator and physical) and run target one <br/>npm run start<br/>npm install<br/>Open dev menu on Android device(adb shell input keyevent 82)<br/>forward android device request to dev machine(adb reverse tcp:8081 tcp:8081)<br/>Android Reloading JavaScript<br/>open React Native debugger ui(Chrome browser required)<br/>react-native log-android<br/>react-native log-ios<br/>gradlew assembleRelease<br/>react-native bundle --platform android/ios --dev false<br/>yarn<br/>jest<br/>react-native uninstall<br/>react-native start<br/>gradlew clean<br/>react-native react-native-git-upgrade<br/>yarn add project, dev, global dependencies<br/>npm add project, dev, global dependencies<br/>auto install and run react-devtools<br/>Last Edit Location(main toolbar)<br/>Reveal file in Finder/Explorer(main toolbar)<br/>Reveal project folder in Finder/Explorer<br/><br/>
New: one-click rerun commands, reuse console window, tabs with title and icon, search in console output.<br/>
Auto detect React Native package.json or build.gradle in current folder and parent/children folder(eg only coding Java in Android Studio),
thus the command will auto execute in the correct folder<br/>



>————— Below is Chinese introduction —————

##功能



一键运行下列功能:<br/>

运行 React Native Debugger https://github.com/jhen0409/react-native-debugger(仅支持Mac)列出并执行package.json中的scripts定义<br>

react-native run-android<br/>
react-native link<br/>
react-native run-ios<br/>
一键真机运行<br/>
列出所有iOS设备(包括模拟器和真机设备)并选中运行<br/>
npm run start<br/>
npm install<br/>
安卓设备上打开开发菜单(adb shell input keyevent 82)<br/>
安卓设备网络请求转发到开发机(adb reverse tcp:8081 tcp:8081)<br/>
安卓设备重新载入JavaScript<br/>
打开 React Native debugger ui(需要Chrome浏览器)<br/><br/>
react-native log-android<br/>
react-native log-ios<br/>
gradlew assembleRelease<br/>
react-native bundle --platform android/ios --dev false<br/>
yarn<br/>
jest<br/>
react-native uninstall<br/>
react-native start<br/>
gradlew clean<br/>
react-native react-native-git-upgrade<br/>
yarn 添加项目, 开发和全局依赖<br/>
npm 添加项目, 开发和全局依赖<br/>
自动安装运行 react-devtools<br/>

最近编辑位置(主工具栏)<br/>
在Finder/Explorer中显示文件(main toolbar)<br/>
在Finder/Explorer中显示项目目录<br/>
指定JS项目工作目录, 例如 ./jsapp, 通过欢迎屏幕或者工具栏按钮 (**可选**, 设置后在.idea目录创建文件 `.rnconsole` , 内容和下面类似:

```json
{
  currentPath: './jsapp'
}
```

之后所有的 npm 命令都会用这个目录作为启动目录<br/>
<br/>

最近更新: 指定JS项目工作目录, 例如 ./jsapp, 可通过欢迎屏幕或者工具栏按钮来完成.<br/>

自动在当前目录和父级目录检测 React Native的package.json文件位置(比如在Android Studio中只开发Java代码时), 这样所有的npm相关的命令都会自动在正确的目录执行<br/>



##Contributors



https://github.com/beansoftapp beansoft@126.com

https://github.com/troublediehard dmportenko@gmail.com

## ScreenShot

![](https://plugins.jetbrains.com/files/9564/screenshot_17784.png)

## Demo Gif
![](https://raw.githubusercontent.com/beansoftapp/react-native-console/master/screenshot/rnconsole.gif)


