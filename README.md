# GalgameTiankeng
樱之诗、最果、Forest、俺翼、灰色、神树之馆、霞外笼等日语白学Galgame汉化天坑的机翻教程和文本

重要的事说三遍：

**这是机翻！**

**这是机翻！**

**这是机翻！**

因此没有占坑之意，只是个人推Gal需要的产物。

# 天坑系列
| 名字                                     | 解包进度 | 机翻进度 | 改错进度 | 加密进度 | 说明                                                         |
| ---------------------------------------- | -------- | -------- | -------- | -------- | ------------------------------------------------------------ |
| 最果てのイマ                             | ×        |          |          |          | 技术无果，联系汉化组中                                       |
| 樱之诗 サクラノ詩 －櫻の森の上を舞う－   | √        | √        |          |          | animed +ScriptDecoder 1000字长请求                           |
| Forest                                   | √        | √        |          | √        | crass gsc剧本 lnedit.exe utf-16编码                          |
| 霞外籠逗留記                             | √        | √        |          | √        | crass gsc剧本 lnedit.exe utf-16编码  *当年好像有人尝试汉化过这部游戏，不过回想里全是乱码；现在已经完全找不到汉化补丁的相关信息了。* |
| 神樹の館                                 | √        | √        |          | √        | crass txt剧本 分割合并^英文                                  |
| 灰色的果实……系列                         |          |          |          |          |                                                              |
| 俺たちに翼はない 我们没有翅膀            | √        | √        |          |          | Lucifen引擎 卡在sob脚本:一个主页的小代码。另外，有公布了文本但是没有补丁。 |
| 俺たちに翼はない 我们没有翅膀 Prelude    | √        | √        |          |          | Lucifen引擎 同上                                             |
| 俺たちに翼はない 我们没有翅膀 AfterStory | √        | √        |          |          | tob脚本，剧本结构也不一样                                    |
| I/O                                      |          |          |          |          |                                                              |


# 个人兴趣、其他系列
| 名字                                  | 解包进度 | 机翻进度 | 改错进度 | 加密进度 | 说明                                                         |
| ------------------------------------- | -------- | -------- | -------- | -------- | ------------------------------------------------------------ |
| 夜行侦探×                             | ×        | ×        |          |          | >没有汉化，关键是找不到程序猿                                |
| FLOWERS -Le volume sur hiver-（冬篇） | √        | √        |          |          | arc_conv + chinesize的getstring带-x参数 500字长请求 enigma壳制作。预定官中，没耐心等。 |
| 崩壊天使アストレイア ×                | ×        | ×        |          |          |                                                              |
| 被黑暗洗礼的天使系列 ×                | ×        | ×        |          |          |                                                              |
| あの晴れわたる空より高く              |          |          |          |          | 好像被KFC接手了                                              |
| 皇姬FD                                | √        | √        |          |          | 有正规组接手，我只是拿来练手的，不封包不做补丁不占坑。       |



TextToUtf-8.py : 大部分剧本拆出来是shift-jis，需要转成最通用的utf-8

TransGalDirText.py : 翻译核心部分代码，使用百度翻译，自动分割字长和按定时发送post

CRLFSplitMerge.py : 针对剧本txt有多行CRLF，建立索引分割避免在线翻译换行符个数不符合

FormatSplitMerge.py : 针对文本句子前后一些固定的符号，建立索引分割避免在线翻译造成结果不符合

文件→脚本+剧本(神樹の館).py : 针对脚本融合在一起的剧本，建立索引分割避免在线翻译造成结果不符合

文件←脚本+剧本(神樹の館).py : 针对脚本融合在一起的剧本，建立索引分割避免在线翻译造成结果不符合

TextToUtf-16.py : 如果需要封包，你可能要先转成utf-16