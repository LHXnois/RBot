# RBot 使用指南

在群聊中发送`使用指南`可快速查看Bot使用指南

## 目录
* [管理](#管理)
    * [模块控制](#模块控制)
    * [Yobot管理](#Yobot管理)
    * [服务器检查](#服务器检查)
    * [广播](#广播)
    * [反并发](#反并发)
    * [轻量群管](#轻量群管)
* [会战](#会战)
    * [Yobot会战](#Yobot会战)
    * [合刀计算](#合刀计算)
    * [实时公会排名](#实时公会排名)
    * [会战报告](#会战报告)
    * [公会人员公开黑名单](#公会人员公开黑名单)
* [聊天](#聊天)
    * [使用指南](#使用指南)
    * [群管](#群管)
    * [问答](#问答)
    * [睡眠套餐](#睡眠套餐)
    * [海豹杀手](#海豹杀手)
    * [语言库](#语言库)
* [娱乐](#娱乐)
    * [Yobot娱乐](#Yobot娱乐)
    * [群空调](#群空调)
    * [骰子](#骰子)
    * [惠惠爆裂魔法](#惠惠爆裂魔法)
    * [表情包生成器](#表情包生成器)
    * [文章生成器](#文章生成器)
    * [发病小作文](#发病小作文)
    * [网抑云](#网抑云)
    * [点歌](#点歌)
    * [报时](#报时)
    * [午间音乐](#午间音乐)
    * [切噜语](#切噜语)
    * [模拟抽卡](#模拟抽卡)
    * [每日签到](#每日签到)
    * [角色语音](#角色语音)
    * [GIF倒放](#GIF倒放)
    * [色图](#色图)
    * [今天也是少女](#今天也是少女)
    * [翻译](#翻译)
    * [今天吃什么](#今天吃什么)
    * [整点报时](#整点报时)
* [游戏](#游戏)
    * [猜头像](#猜头像)
    * [猜角色](#猜角色)
    * [猜语音](#猜语音)
    * [猜现实](#猜现实)
    * [猜群友](#猜群友)
    * [猜up](#猜up)
    * [猜邦邦](#猜邦邦)
    * [贵族决斗](#贵族决斗)
    * [赛跑](#赛跑)
    * [模拟赛马](#模拟赛马)
    * [俄罗斯轮盘](#俄罗斯轮盘)
* [查询](#查询)
    * [Yobot查询](#Yobot查询)
    * [公主连结资料查询](#公主连结资料查询)
    * [天气查询](#天气查询)
    * [搜图搜番](#搜图搜番)
    * [B站动态](#B站动态)
    * [无损音乐搜索](#无损音乐搜索)
    * [Rank表](#Rank表)
    * [Pcr活动日历](#Pcr活动日历)
    * [新闻推送](#新闻推送)
    * [漫画推送](#漫画推送)
    * [定时提醒](#定时提醒)
* [未启用插件](#未启用插件)
    * [授权管理](#授权管理)
    * [P站搜图](#P站搜图)
    * [Hoshino会战](#Hoshino会战)
    * [Hoshino报告](#Hoshino报告)
    * [在线色图](#在线色图)





## 管理
### 模块控制
Bot 的功能繁多，可根据自身需要控制开关，在群聊中发送 `lssv` 即可查看各功能模块的启用状态，使用以下命令进行控制：
```
启用 service-name
禁用 service-name
```
为防止单条消息过长，每项功能的指令说明分别显示。使用以下命令可以查看各项功能的说明：
```
service-name帮助
```

### Yobot管理
| 指令 | 说明 |
| --- | --- |
|登录|	登录进入 Web 模式
|重置密码|	随机重置一个新密码
|更新|	(权)更新机器人
|重启|	(权)重新启动机器人
|退出此群|	(权)命令机器人退出当前群聊
|version|	查看机器人版本

### 服务器检查
| 指令 | 说明 |
| --- | --- |
| @bot 服务器检查 | 查看服务器详细信息（需主人权限）
| @bot 服务器状态 | 查看服务器简略信息（需主人权限）


### 广播
| 指令 | 说明 |
| --- | --- |
| 广播 XX | 将内容广播至所有群（需主人权限）

### 反并发
[anticoncurrency - 反并发](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/anticoncurrency)

### 轻量群管
[Groupmaster - 轻量群管](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/groupmaster)



## 会战
### Yobot会战
| 指令 | 说明 |
| --- | --- |
|手册	|查看公会战使用手册
|面板	|进入公会战面板
|创建X服公会	|
|加入公会 [@某人]	|加入到公会名单，如果有 at 则为加入他人
|加入全部成员	
|报刀2000000 [@某人] [昨日] [:留言]	|对boss造成伤害但未击败时用，记录伤害，可以使用 200w/200万/2000k 等，如果有at则为代报，如果有“昨日”则将记录添加到前一天
|尾刀 [@某人] [昨日] [:留言]	|对 boss 造成伤害并击败时用，记录伤害，如果有 at 则为代报，如果有“昨日”则将记录添加到前一天
|SL [？]	|挑战 boss 强制取消后用，记录本日 SL，用“？”查询今日是否已 SL
|撤销	|撤销上一次报刀（非管理员只能撤销自己的记录）
|状态	|显示 boss 状态
|预约1 [:留言]	|预约 boss，当 boss 出现时通知
|挂树 [:留言]	|挂树，当 boss 被击败时通知
|查1 / 查树	|查询预约 boss 的成员，查询挂树的成员
|取消预约1 / 取消1	|取消预约
|申请出刀	|锁定 boss，提醒后面的人有人正在挑战 boss
|锁定:留言	|锁定 boss，提醒后面的人暂停出刀，冒号后为留言
|解锁	|解锁 boss，其他人可以继续申请
|(后台：出刀表)	|查看所有成员当时出刀情况与SL情况，也可以查看过去的出刀信息
|(后台：催刀)	|at并提醒所有未完成出刀的成员
|(后台：尾刀信息)	|查看所有有剩余刀的成员的上一次尾刀信息
|(后台：修改boss状态)	|boss数据与实际情况不一致时进行修改
|(后台：重置数据)	|两次公会战之间使用，删除所有出刀、预约数据

### 合刀计算
| 指令 | 说明 |
| --- | --- |
|合刀 刀1伤害 刀2伤害 剩余血量| 计算合刀补偿时间

### 实时公会排名
| 指令 | 说明 |
| --- | --- |
|绑定公会 会长ID | 绑定本群公会
|公会排名 | 查询本群公会排名
|分数线 | 查询分数线
|查询会长 ABC |查询会长名字包含ABC的公会的排名
|查询公会 ABC |查询公会名字包含ABC的公会的排名
|查询排名 5000 | 查看5000名的公会分数信息

### 会战报告
|指令|说明|
|-----|-----|
|生成会战/离职报告| 生成本人报告
|生成会战/离职报告  @用户| 生成他人报告
|设置工会api 地址  |(需要管理员权限)为本群设置默认的Yobot工会API
|查看工会api| (需要管理员权限)查看本群设置的Yobot API
|清除工会api| (需要管理员权限)清除本群设置的Yobot API

### 公会人员公开黑名单
| 指令 | 说明 |
| --- | --- |
|失信 123456789 | 根据UID或者QQ号搜索





## 聊天
### 使用指南
| 指令 | 说明 |
| --- | --- |
| 使用指南 | 查看Bot使用说明
| 帮助 | 查看Yobot功能列表
| 指令表 | 查看各功能指令示例
| 更新日志 | 查看bot更新日志
| 来杯咖啡 XX | 反馈内容 联系bot主人

### 群管
| 指令 | 说明 |
| --- | --- |
|申请头衔XX	|XX为头衔名
|删除头衔	|删除自己获得的头衔,可以@其他人
|禁言@sb XX	|xx为秒数
|解除禁言@sb	|字面意思
|全员禁言	|开启全员禁言
|飞机票@sb	|把sb请出本群
|设置管理员 @sb	|
|取消管理员 @sb	|
|修改名片@sb xxx	|把sb的群名片设置为xxx
|发送群公告 XXX	|
|@bot说 XX	|bot语音

### 问答
| 指令 | 说明 |
| --- | --- |
|大家说111回答222|对所有人生效
|我说333回答444|仅对个人生效
|问答|查看自己的回答
|问答@某人|查看别人的回答
|不要回答111|删除某问题下的回答(优先度:自己设置的>最后设置的)
|清空回答111|清空一个问答
|全部问答|显示本群所有的问答

### 睡眠套餐
| 指令 | 说明 |
| --- | --- |
|精致睡眠|	8小时精致睡眠(bot需具有群管理权限)
|给我来一份精致昏睡下午茶套餐|	一杯先辈特调红茶(bot需具有群管理权限)

### 海豹杀手
|指令|说明|
|-----|-----|
|启用海豹杀手 [海豹判定阈值]|在当前群启用海豹杀手插件。如果不输入参数，默认阈值是100抽，小于100抽出货的均判定为海豹|
|禁用海豹杀手|在当前群禁用海豹杀手插件|

### 语言库
[Botchat - 轻量语言库](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/botchat)

## 娱乐
### Yobot娱乐
| 指令 | 说明 |
| --- | --- |
|十连	|模拟抽卡
|仓库[@某人[@某人[…]]]	|查看抽到过的所有角色查看他人抽到过的角色
|在线十连	|在线抽卡，不扰民
|人偶	|(权:主人)人偶功能

### 群空调
| 指令 | 说明 |
| --- | --- |
| 开空调 |	打开空调（第一次使用时会自动安装空调）
| 关空调 |	关闭空调
| 当前温度 |	查看当前风速、设定温度、环境温度
| 设置温度 <温度>	| 设置空调温度
| 设置风速 <1/2/3> (或者低/中/高) |	设置空调风速（共有三档）
| 设置环境温度 <温度>	| 设置环境温度
| 升级空调	| 升级空调（家用空调👉中央空调）
| 降级空调	| 降级空调（中央空调👉家用空调）
| 空调类型	| 查看空调类型（家用空调/中央空调）

### 骰子
| 指令 | 说明 |
| --- | --- |
|.r	| 掷1次100面骰子
|.r 3d12	|掷3次12面骰子

### 惠惠爆裂魔法
| 指令 | 说明 |
| --- | --- |
|爆裂魔法| 和惠惠随机练习一发爆裂魔法
|@bot 补魔| 补充魔力（重置每日上限）

### 表情包生成器
| 指令 | 说明 |
| --- | --- |
|表情列表|	查看目前有哪些表情
|生成表情 表情名字 文案|	生成一张表情包
|查看表情 XXX|	XXX是表情名字,要准确
|查看XX表情|	XX是表情名字的关键词,支持模糊搜索
|删除表情 XX|	XX是表情名字
|上传表情 表情名字 图片|	上传一张表情

### 文章生成器
| 指令 | 说明 |
| --- | --- |
|营销号 主体/事件/另一种说法|	营销号生成器
|狗屁不通 主题|	狗屁不通生成器
|记仇 天气/主题|	记仇表情包生成器
|我朋友说他好了|	无中生友，无艾特时随机群员
|日记 天气/主题|	舔狗日记生成器

### 发病小作文
| 指令 | 说明 |
| --- | --- |
|发病 对象|	发送一篇写给对象的发病小作文
|小作文|	随机发送一篇库存发病小作文
|病情加重 对象/小作文|	将一篇发病小作文添加到数据库中

### 网抑云
| 指令 | 说明 |
| --- | --- |
|上号/网抑云/到点了 |	生成网抑云语录

### 点歌
| 指令 | 说明 |
| --- | --- |
|点歌 好日子	|混合搜索
|搜网易云 好日子|	搜索网易云
|搜QQ音乐 好日子|	搜索QQ音乐
|搜咪咕音乐 好日子|	搜索咪咕音乐

### 报时
| 指令 | 说明 |
| --- | --- |
|报时	|生成一张报时图

### 午间音乐
|指令|说明|
|-----|-----|
|来点音乐|随机推送一首公主连结相关音乐|
|来点音乐 [关键词]|寻找活动名/歌曲名含有关键词的音乐并推送|

### 切噜语
|指令|说明|
|-----|-----|
|切噜一下 XX|	转换为切噜语
|切噜～♪XX|	切噜语翻译

### 模拟抽卡
|指令|说明|
|-----|-----|
|@bot 来发十连|  模拟十连抽奖
|@bot 来发单抽| 模拟单抽
|@bot 来一井|  模拟4w5一井
|查看卡池| 查看当前模拟卡池信息
|切换卡池| 更换模拟卡池
|氪金@xxx| 群管理使用此指令来重置抽卡次数限制，可@多人
|更新卡池| 更新卡池, 仅限超级管理员, 可群聊可私聊, 无需@, 无需开启服务
|选择卡池| 与原指令相同, 请根据提示操作

### 每日签到
|指令|说明|
|-----|-----|
|@bot 签到| 

### 角色语音
|指令|说明|
|-----|-----|
|XX语音|随机播放一段XX角色语音|

### GIF倒放
|指令|说明|
|-----|-----|
|倒放 xxx.gif| 附带GIF图 

### 色图
|指令|说明|
|-----|-----|
|色图/涩图/不够色/...|随机发送一张色图
|换肾/换弹夹 @用户| 重置每日上限

### 今天也是少女
|指令|说明|
|-----|-----|
|今天我是什么少女| 查看自己
|今天你是什么少女 @用户| 查看别人

### 翻译
|指令|说明|
|-----|-----|
|翻译 原文| 

### 今天吃什么
| 指令 | 说明 |
| --- | --- |
|[今天/早上/中午/晚上/夜宵][吃][什么/啥]|

### 整点报时
[Hourcall - 整点报时](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/hourcall)





## 游戏
### 猜头像
| 指令 | 说明 |
| --- | --- |
|猜头像 |	猜猜机器人随机发送的头像的一小部分来自哪位角色
| 猜头像群排行	| 显示猜头像小游戏猜对次数的群排行榜(只显示前十名)

### 猜角色
| 指令 | 说明 |
| --- | --- |
|猜角色 |	猜猜机器人随机发送的文本在描述哪位角色
| 猜角色群排行	| 显示猜角色小游戏猜对次数的群排行榜(只显示前十名)

### 猜语音
| 指令 | 说明 |
| --- | --- |
| cygames |	猜猜机器人随机发送的"cygames"语音来自哪位角色
| 猜语音 |	猜猜机器人随机发送的语音来自哪位角色
| 猜语音群排行 | 显示猜语音小游戏猜对次数的群排行榜(只显示前十名)

### 猜现实
| 指令 | 说明 |
| --- | --- |
| 猜现实 |	猜猜机器人随机发送的现实图片是哪位角色
| 猜现实群排行	| 显示猜现实小游戏猜对次数的群排行榜(只显示前十名)

### 猜群友
| 指令 | 说明 |
| --- | --- |
|猜群友 |	猜猜机器人随机发送的头像的一小部分来自哪位群友

### 猜up
| 指令 | 说明 |
| --- | --- |
| 猜up |	猜猜机器人随机发送的头像的一小部分来自哪位vup
| 猜up群排行 | 显示猜up小游戏猜对次数的群排行榜(只显示前十名)

### 猜邦邦
| 指令 | 说明 |
| --- | --- |
|猜邦邦 |	猜猜机器人随机发送的头像的一小部分来自哪位邦邦角色
| 猜邦邦群排行	| 显示猜邦邦小游戏猜对次数的群排行榜(只显示前十名)

### 贵族决斗
| 指令     | 说明     |
| ------------- | -------------|
|创建贵族       | 可以在本群创建自己的贵族，会被随机分配一个女友。       |  
|查询贵族(@成员) |可以查询自己或群友的贵族状态。
|贵族约会/招募女友 |可以花费500金币招募一个女友，女友数不能超过爵位上限。
|升级贵族/升级爵位 |可以花费金币提升自己的爵位,提升爵位时女友数需已达到上限。
|贵族决斗+@成员（强制） |可以向另一个贵族发起决斗，两个人必须都是贵族且已拥有女友，输者会随机被抢走一个女友。带强制时，使用强制决斗卡道具
|领金币 |可以在金币归零时领取150金币。
|查金币 |可以查询自己现在的金币数。
|贵族签到 |可以领取金币和声望，数量与爵位和运气有关。
|为(用户qq)充值xx金币 |可以为该用户充值金币
|重置决斗 |可以解锁决斗开关。(限管理员以上，这个仅用于决斗卡死无法再开的时候)
|查女友+角色名 |可以查询某位角色的归属。
|分手+角色名 |可以和角色分手(需要支付分手费和声望)。
|贵族帮助 |可以查看游戏说明书。
|dlc帮助 |可以查看dlc系统功能
|本群贵族 |可以查看本群贵族统计，剩余女友，及加载dlc的状况
|加冕称帝 |可以由国王提升至皇帝
|飞升成神 |可以由皇帝提升至神
|贵族等级表 |可以查看贵族提升消耗及权利
|为@某人转账xxx金币 |用以向某人转账金币，需要扣除手续费
|用xxx金币与@qq交易女友+角色名|进行女友交易，需要扣除买入方的声望，需要扣除手续费
|声望/金币/女友排行|查看排行榜
|查询庆典|查看目前正在进行的庆典状况
|梭哈支持XX号|是男人就梭哈！投入所有的金币支持某位选手
|扣除QQ号的XXX声望|特殊情况用，扣除某人声望
|声望招募|使用声望必定招募女友
|免费招募|免费招募必定招募一名女友
|皇室婚礼+角色名|和一名角色结婚
|离婚+角色名|和自己的妻子离婚
|确认重开|删除自己的角色，从头再来
|重置角色qq|删除一名玩家的数据库，令其重新开始
|重置金币qq|清空一名玩家的金币
|设定群XXX为X号死|操盘（这个功能十分无聊，但可以防止人脱坑）
|初始化本群庆典|按照配置内的设置，快速初始化本群庆典
|开启/关闭本群XX庆典|群内开关庆典
|好感帮助|可以查看好感系统帮助
|购买上限 |可以增加女友上限(国王以上可用)
|贵族婚礼+角色名 |可以拥有第二名妻子（神可用）
|武器列表|查看本群可用武器（仅供娱乐）
|切换武器XXX|切换本群武器
|贵族胜场排行|查看胜场排行
|送发情蛋糕XXX|测试用，提升某角色300好感度
|真步真步|测试用，增加10胜场
|封停/解封群XXX的XXX号|封号系统，有钻空子的封了他
|发放补偿XXX个(金币/声望/公主之心)|为当前全群发放补偿（公主之心是补20好感的道具，可以改成别的）
|本群重开|本群删库，请小心误操作，默认重开后补偿5000X等级金币，300X等级声望，和X等级公主之心
|开启/关闭（或查询）本群不决斗惩罚|开关本群不决斗惩罚
|清空群XXX的XXX的认输场次|清空认输场次
|为XXX发放XXX个XXX|为某人发礼物
|神秘商店|查看当前的神秘商店商品
|购买物品 X|购买神秘商店物品
|批量送礼 数量 女友名 礼物名|批量送礼功能
|使用道具 道具名 目标名|使用道具
|升级称号|提升称号等级
|查询道具|查询各自道具的效果及持有数

### 赛跑
|指令|说明|
|-----|-----|
|测试赛跑|刷屏警告（需管理权限）|
|赛跑排行榜|查询本群赛跑金币排行|
|重置赛跑|重置赛跑（需管理权限）|

### 模拟赛马
|指令|说明|
|-----|-----|
|@bot 赛马开始| 

### 俄罗斯轮盘
|指令|说明|
|-----|-----|
|俄罗斯轮盘| 开始俄罗斯轮盘赌游戏

## 查询
### Yobot查询
| 指令 | 说明 |
| --- | --- |
|jjc查询 A B C D E	|查找竞技场解法，指定区服可改用“jjc国服/jjc台服/jjc日服”
|日程(今日/明日/x月x日)(可自动)	|查看活动日程
|日程表	|查看一周日程
|挖矿计算 当前名次	|计算剩余可获得的奖励钻

### 公主连结资料查询
|指令|说明|
|-----|-----|
| 挖矿 名次 | 竞技场余矿查询
|XX是谁/谁是XX| 角色别称查询
|pcr速查/图书馆| 公主连结资料网站
|bcr速查/攻略| 公主连结攻略
|黄骑充电表|
|一个顶俩/拼音接龙|注音文字拼音对照表
|更多资料|

### 天气查询
| 指令 | 说明 |
| --- | --- |
|查天气|

### 搜图搜番
|指令|说明|
|-----|-----|
|识图/搜图 图片| 以图搜图
|识番/搜番 图片| 以图搜番

### B站动态
| 指令 | 格式 | 备注 |
| ---------- | -------------- | -------------- |
| 订阅动态 | 订阅动态+空格+需要订阅的UID+空格+需要订阅的群（可选） | 如不输入订阅的群则为当前群，全部群订阅请输入all |
| 取消订阅动态 | 取消订阅动态+空格+需要取消订阅的UID+空格+需要取消订阅的群（可选） | 如不输入取消订阅的群则为当前群，取消全部群订阅请输入all |
| 重新载入动态推送配置 | 无 | 在不重载HoshinoBot的情况下重新载入修改后的配置文件 |

### 无损音乐搜索
| 指令 | 说明 |
| --- | --- |
|搜无损 内容| [搜索动漫无损音乐](http://www.acgjc.com/)

### Rank表
| 指令 | 说明 |
| ------ | ------- |
| 日/台/陆rank | 查询rank表 |
| 查看当前rank更新源 | 字面意思 |
| 查看全部rank更新源 | 列出远程rank表更新源 |
| 设置rank更新源 国/台/日 稳定/自动更新 源名称 | 无 |
| 更新rank表缓存 | 手动更新rank表缓存 |

### Pcr活动日历
| 指令 | 说明 |
| ------ | ------- |
|日历 | 查看本群订阅服务器日历
|[国台日]服日历 | 查看指定服务器日程
|[国台日]服日历 on/off | 订阅/取消订阅指定服务器的日历推送
|日历 time 时:分 | 设置日历推送时间
|日历 status | 查看本群日历推送设置
|日历 cardimage | (go-cqhttp限定)切换是否使用cardimage模式发送日历图片

### 新闻推送 
[Priconne-News - 官方新闻推送](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/priconne/news)

### 漫画推送
[Priconne-Comic - 官方四格漫画推送](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/priconne)

### 定时提醒
[Pcrwarn - 定时提醒](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/pcrwarn)



## 未启用插件
### 授权管理
[authMS - 授权管理](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/authMS)（个人使用）

### P站搜图
[epixiv - p站搜图](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/epixiv)（未配置）

### Hoshino会战
[PcrClanbattle - 公会战管理Hoshino版](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/pcrclanbattle/clanbattle)（使用Yobot）

### Hoshino报告
[Report-Hoshino - 会战报告Hoshino版](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/report-hoshino)（使用Yobot）

### 在线色图
[Setu_renew - 在线色图](https://github.com/RMYHY/RBot/tree/main/HoshinoBot/hoshino/modules/setu_renew)（未配置）
