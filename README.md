# FishBotGUI
  
源自 https://github.com/MscBaiMeow/FishBot  (v1.6.0以下) 及 https://github.com/MscBaiMeow/FishBot2  
  
此为[FishBot](https://github.com/MscBaiMeow/FishBot)及[FishBotReload](https://github.com/MscBaiMeow/FishBot2)的GUI版本  
采用~~巨鸡儿烂的~~易语言进行编写，仅可供Windows用户使用  
Linux用户请前往原贴[(旧版本)](https://github.com/MscBaiMeow/FishBot/releases)或[(新版本)](https://github.com/MscBaiMeow/FishBot2/releases)下载`AutoFish`  

## ~~更新延期提示~~存档提示

~~此项目在不久的将来可能会重构。因此更新将可能延期。~~  
新版FishBot2已有可视化ui计划。因此本项目将作存档处理。

## 版本对应说明

| Minecraft版本 | 最后对应GUI版本 | *预计*可用GUI版本 [^1] | 备注 |
|:------:|:---------:|:---------:|:---------:|
| 1.14.4 | ```1.4.2.01``` | 1.1 - 1.4.2.01 ||
| 1.15.2 | ```1.4.4``` | 1.4.3 - 1.5.0 ||
| 1.16.1 | ```1.6.0``` | 1.5.1 - 1.6.0 ||

[^1]：此处为预计可用GUI版本，请以实际情况为准

## 截图 (仅供参考)
![1](https://raw.githubusercontent.com/Amazefcc233/FishBotGUI/master/images/snipaste_20190813_001417.png)
![2](https://raw.githubusercontent.com/Amazefcc233/FishBotGUI/master/images/snipaste_20190813_001716.png)

## Release 注意事项

1. 自**v1.6.0以后**（即从FishBot2新版本开始），版本号将不再与FishBot版本同步。  
   新GUI版本号格式将统一为```2.x.x.x```， 起始位置为```2.1.1.0```。其中：  
   - ```2```为区别于旧版本的标识
   - ```x.x.x```三项分别为```主版本号```、```次版本号```、```修订号```。  
     ~~(简直就是抄了但又没完全抄[语义化版本 2.0.0 规范](https://semver.org/lang/zh-CN/))~~  
     GUI版本的版本号递增规则大致如下：
     - 若FishBotGUI存在巨大变动（通常跟随FishBot进行变动），则通常情况下将递增一次主版本号。
     - 若FishBot主体文件未进行较大变动，则无论FishBot版本号变更为多少，通常情况下GUI版本将递增一次次版本号。
     - 若上一版GUI版本存在问题，而FishBot未出错（或未更新），则递增一次修订号。
     - 当次版本号递增后，修订号将被重置，从0开始重新计算。
     - 当主版本号递增后，次版本号和修订号将被重置，次版本号从1开始重新计算，修订号从0开始重新计算。
   
   在内置的程序版本信息中，将统一为`2.0.0.0`。除非FishBot再次重开仓库，否则以后不再进行更改。
2. 自**v1.6.0以后**（即从最后一版FishBot旧版本后开始），一次Release将会发布两个程序。  
   其中```AutoFishGUI.exe```为包含对应FishBot主体文件的GUI版本，```AutoFishGUI-only.exe```仅有GUI启动界面，实际启动文件需从原帖[(旧版本)](https://github.com/MscBaiMeow/FishBot/releases)或[(新版本)](https://github.com/MscBaiMeow/FishBotReload/releases)下载，并改名为```AutoFish.exe```，将其与```AutoFishGUI-only.exe```放置在同一文件夹下。

## 启动注意事项

1. 在启动后，同目录下将会生成```autofish-gui-auto.bat```文件。若您无需配置上的更改，可直接运行此文件启动钓鱼机。
2. 如想保留原有配置文件，将```autofish-gui-auto.bat```文件改名即可。
3. 服务器ip不可为srv解析。可通过nslookup查看获得a记录地址和端口并重新填入。  
例：服主给出的服务器地址为```mc.example.com```，但通过cmd执行ping命令显示```Ping 请求找不到主机```，或是看得到ping后的ip却仍然无法进入服务器，则可能是使用了srv解析。  
通过输入命令```nslookup -q=srv _minecraft._tcp.mc.example.com```发现，```port```为```10000```，```srv hostname```为```a.example.com```，则可在启动器内服务器ip栏输入```a.example.com```，端口输入```10000```。  
若输入命令后发现```srv hostname```仍然为```mc.example.com```，那么可以```ping mc.example.com```来获取服务器的ip地址，然后填入服务器地址栏并填写端口，即可进入服务器。

### 正版用户须知

1. **从v1.4起，密码将不再被保存在本地，取代而之的是astk。安全性的确有所提高，但请您注意，使用astk登入仍有可能导致您的账户被他人利用。因此在任何时候，您都不应该泄露自己的astk和密码信息。我们已对此进行过警告，因随意传播密码/astk而导致账号被盗等行为，FishBot及FishBotGUI不承担任何责任。**
2. ***这里正版指的是国际服正版。和网易国服没有任何一丁点关系。***
3. 若想加入领域服，只需选择“领域”复选框即可，无需填写ip和端口。在钓鱼机登录后，可选择一个领域服并进入。

### 外置登录用户须知

1. **从v1.4起，密码将不再被保存在本地，取代而之的是astk。安全性的确有所提高，但请您注意，使用astk登入仍有可能导致您的账户被他人利用。因此在任何时候，您都不应该泄露自己的astk和密码信息。我们已对此进行过警告，因随意传播密码/astk而导致账号被盗等行为，FishBot及FishBotGUI不承担任何责任。**
2. 请在认证服务器一栏中填写你服务器的Yggdrasil API 认证服务器地址。
3. 统一通行证用户在认证服务器一栏中填写```https://auth2.nide8.com:233/($服务器ID)/```。```($服务器ID)```为注册URL的32位ID。
  若注册地址为```https://login2.nide8.com:233/1234567890abcdef1234567890abcdef/loginreg```，则服务器id为```1234567890abcdef1234567890abcdef```。
4. 事实上并没有打算考虑统一通行证。能用便是缘分。用不了也不打算兼容。
5. 多用户可在钓鱼机登入后选择一个用户并进入服务器。

### 中国版用户须知

1. 根据推断，无论是租赁服还是网络服，中国版都有其自己开发的认证渠道，且相关核心也有经过相关工作组二次开发。因此除非有他人破解或自行公开相关源码，否则通常情况下无法以非官方方式登录。

## 鸣谢

- [go-mc](https://github.com/Tnze/go-mc)
- [FishBot](https://github.com/MscBaiMeow/FishBot)
- [Miaoscraft](https://github.com/miaoscraft/)
- [易语言 - 未闻花名UI](https://bbs.125.la/home.php?mod=space&uid=378021)
- [Tsuk1ko/CQ-picfinder-robot的模版](https://github.com/Tsuk1ko/CQ-picfinder-robot)
