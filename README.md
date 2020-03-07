# electron_nsis_UI
Niuniu_NSIS_SetupSkin

## 打包前的准备
- 将 electron-web 项目 builder 后 dist/win-unpacked 下的文件及文件夹放到 FilesToInstall 文件夹内

## 配置
- 修改 SetupScripts/bszs/bszs_demo.nsi 文件的 EXE_NAME 属性值为上一步操作的 exe 文件名

## 打包
- 直接执行 build-bszs.bat 文件即可

## 安装文件
- 位于 Ouput 文件夹内，双击安装