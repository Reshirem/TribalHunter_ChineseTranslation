# TribalHunter_ChineseTranslation
部落猎人 文本汉化

## 关于项目
看到这款游戏还没有汉化补丁，所以尝试做一次汉化。

这款游戏汉化难点主要是字库问题，爬坑花了一段时间，基本算是解决了。（以后工具更新后大概就不算难点了吧23333）

还有个难点在于这英语对我来说太难了，所以想有个能帮忙润色文本的就更好了。

等这游戏出了韩文之后，估计汉化字体就能轻松和英文字体分开了。要是GMS2支持一个字库内塞多个字体就好了，用PS好麻烦哦。

不会发布已经打包好的资源文件，因为资源文件就相当于游戏本体了，发出来始终不合适。也许以后会制作补丁工具，或者跟作者联系变成官中。

## 使用方法
1. 工具的准备

   拉取并编译运行UndertaleModTool（后面都称之为UMT）的[gms-2.3.1-read-only-version](https://github.com/krzys-h/UndertaleModTool/tree/gms-2.3.1-read-only-version)分支。
   
   也可以使用Grossley写的[underfell-test](https://github.com/Grossley/UndertaleModTool/tree/underfell-test)分支。
   
   二选一。
   
2. 获取字库和文本

   暂时不想写具体，是直接下载还是用git拉取都没所谓，反正能运行工具的话应该都知道怎么做了。
   
3. 汉化

   把游戏根目录内的data.win复制多一份副本，然后使用UMT读取复制出来的副本！再使用工具里的FontDataImport.csx。
   
   ![image](https://user-images.githubusercontent.com/12333564/113618690-9c7ca600-968a-11eb-94bd-32b39aff0c43.png)
   
   弹出路径选择的窗口后，选择到下载下来的字库文件夹内（Export_Fonts），然后点击打开。
   
   ![image](https://user-images.githubusercontent.com/12333564/113618648-8ff84d80-968a-11eb-96b4-76aa44105b08.png)
   
   然后会显示导入成功。
   
   ![image](https://user-images.githubusercontent.com/12333564/113618714-a4d4e100-968a-11eb-82af-4bbd5f59803f.png)
   
   然后保存所作出的修改，也许会遇到报错所以禁用保存的情况，反正关闭工具的时候都会询问你是否要保存改动。保存得到的data.win替换原有的就行了。
   
   ![image](https://user-images.githubusercontent.com/12333564/113618765-b4ecc080-968a-11eb-888a-18fdbc657f3e.png)
   
   最后把下载下来的汉化文本（Resources文件夹）覆盖到游戏根目录即可。（备份嘛，反正校验游戏就恢复了，我觉得没必要）
   
   ![image](https://user-images.githubusercontent.com/12333564/113618852-cc2bae00-968a-11eb-9fc5-fddb1855ace3.png)
   
   然后就可以启动游戏测试啦。
   
   ![image](https://user-images.githubusercontent.com/12333564/113619059-144ad080-968b-11eb-833f-b4de01d8bfeb.png)

   ![image](https://user-images.githubusercontent.com/12333564/113619217-4c521380-968b-11eb-87b8-9e5abf009519.png)


## 关于字库生成
先简单写写方便有兴趣的朋友测试。

使用2.1.5版本的GameMaker: Studio，创建一个项目，创建字体（字体名要对应要替换的字体，字体名参考UMT打开data.win时候的Fonts树），在添加里从文件导入要添加的字体（我试过生成6万个字符等3个小时都没结果），之后按Ctrl+F8生成为Zip格式，解压后可以得到一个包含你创建的字体的data.win，用UMT打开后用FontDataExport.csx导出字体即可。

## Todo
- [ ] 找个更合适的字体
- [ ] 针对不同地方使用不同的字体
- [ ] 还有吗？

## 汉化进度
更新时间: 2021/04/06

文件名 | 进度
------|:------:
scrDataBoss | 未开始
scrDataCinem | 机翻95%
scrDataMaps | 机翻95%
scrDataMenu | 机翻85%
scrDataNPCchat | 机翻60%
scrDataTLBeach | 未开始
scrDataTLCastle | 润色0%
scrDataTLCrystal | 未开始
scrDataTLGhost | 未开始
scrDataTLHive | 未开始
scrDataTLJungle | 未开始
scrDataTLMountain | 未开始
scrDataTLPiglands1 | 未开始
scrDataTLSlime | 未开始
scrDataTLVillage | 机翻5%
scrDataTriggerBeach | 未开始
scrDataTriggerCastle | 未开始
scrDataTriggerCrystal | 未开始
scrDataTriggerGhost | 未开始
scrDataTriggerHive | 未开始
scrDataTriggerJungle | 未开始
scrDataTriggerMountain | 未开始
scrDataTriggerPiglands1 | 未开始
scrDataTriggerSlime | 润色0%
scrDataTriggerVillage | 未开始
scrDataTV | 未开始

## 爬坑过程
https://redoru.cn/?p=13
