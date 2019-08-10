# FishBotGUI
  
源码 https://github.com/MscBaiMeow/FishBot  
  
此为[FishBot](https://github.com/MscBaiMeow/FishBot)的GUI版本  
采用~~巨鸡儿烂的~~易语言进行编写，仅可供Windows用户使用  

## Release 注意事项

1. 每次的Release中，**大概**会有两个文件。  
  一个是```AutoFishGUI.exe```，另一个是```AutoFishGUI-small.exe```。  
  两者的区别就在于，前者已包含了主文件，后者仅包含GUI启动部分，您必须手动下载[FishBot](https://github.com/MscBaiMeow/FishBot/releases)中的版本，并将其和GUI启动器放置在同一目录下，才可启动钓鱼机。
2. 本GUI的release版本将跟随FishBot版本。

## 启动注意事项

1. 在启动后，同目录下将会生成```autofish-gui-auto.bat```文件。若您无需配置上的更改，可直接运行此文件启动钓鱼机。
2. 如想保留原有配置文件，将```autofish-gui-auto.bat```文件改名即可。

### 正版用户须知

1. **您的密码将以明文方式保存在本地，即```autofish-gui-auto.bat```文件中。切记不要将此文件随意发送给其他人，否则可能会导致你的账号和密码被泄露。我们已对此进行过警告，因随意传播密码而导致账号被盗等行为，FishBot及FishBotGUI不承担任何责任。**
2. ***这里正版指的是国际服正版。和网易国服没有任何一丁点关系。***

### 外置登录用户须知

1. **您的密码将以明文方式保存在本地，即```autofish-gui-auto.bat```文件中。切记不要将此文件随意发送给其他人，否则可能会导致你的账号和密码被泄露。我们已对此进行过警告，因随意传播密码而导致账号被盗等行为，FishBot及FishBotGUI不承担任何责任。**
2. 请在认证服务器一栏中填写你服务器的Yggdrasil API 认证服务器地址。
3. 统一通行证用户在认证服务器一栏中填写```https://auth2.nide8.com:233/($服务器ID)/```。```($服务器ID)```可为注册URL的32位ID。
  若注册地址为```https://login2.nide8.com:233/1234567890abcdef1234567890abcdef/loginreg```，则服务器id为```1234567890abcdef1234567890abcdef```。
4. ***很抱歉，我们暂不支持外置登录。~~我们什么也不会做的。~~***

## 鸣谢

- [go-mc](https://github.com/Tnze/go-mc)
- [FishBot](https://github.com/MscBaiMeow/FishBot)
- [Miaoscraft](https://github.com/miaoscraft/)
