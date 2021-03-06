介绍
===================
> - **Created time: 06/21/2017**
> - **Author: Cain Li**
===================

发牌一般分为5个步骤，分别为：

Perflop — 先下大小盲注，然后给每个玩家发2张底牌，大盲注后面第一个玩家选择跟注、加注或者盖牌放弃，按照顺时针方向，其他玩家依次表态，大盲注玩家最后表态，如果玩家有加注情况，前面已经跟注的玩家需要再次表态甚至多次表态。

Flop — 同时发三张公牌，由小盲注开始（如果小盲注已盖牌，由后面最近的玩家开始，以此类推），按照顺时针方向依次表态，玩家可以选择下注、加注、或者盖牌放弃。

Turn — 发第4张牌，由小盲注开始，按照顺时针方向依次表态。

River — 发第五张牌，由小盲注开始，按照顺时针方向依次表态，玩家可以选择下注、加注、或者盖牌放弃。

===================

同花大顺（Royal Flush）：最高为Ace（一点）的同花顺。

同花顺（Straight Flush）：同一花色，顺序的牌。

四条（Four of a Kind，亦称“铁支”、“四张”或“炸弹”）：有四张同一点数的牌。

满堂红（Fullhouse，亦称“俘虏”、“骷髅”、“夫佬”、“葫芦”）：三张同一点数的牌，加一对其他点数的牌。

同花（Flush，简称“花”：五张同一花色的牌。

顺子（Straight，亦称“蛇”）：五张顺连的牌。

三条（Three of a kind，亦称“三张”）：有三张同一点数的牌。

两对（Two Pairs）：两张相同点数的牌，加另外两张相同点数的牌。

一对（One Pair）：两张相同点数的牌。

高牌（high card）：不符合上面任何一种牌型的牌型，由单牌且不连续不同花的组成，以点数决定大小。

===================

庄家           button

小盲注         smallBlind

大盲注         bigBlind

筹码           jetton

金币           money

奖池所有筹码    pot

投注额         bet

===================

-- 数据结构
1. 建立玩家自己的数据结构
2. 创建对历史所有动作的保存表，如对手每一阶段的加注，跟注，弃牌等，返回概率(阈值)
3. 工具类，作牌的大小对比，牌类型的判断
4. 算概率的方法

-- 大致逻辑
1. 如果所有对手都已经弃牌了，叫注
2. 如果自己的筹码远远超出对手，则让牌或弃牌
3. 如果还有没弃牌的对手，根据目前属于哪个环节，并根据自己手牌估算综合概率(阈值)
4. 根据概率判断是否加注/让牌/跟牌/弃牌

=====================

洗牌 Shuffle,
发牌 Deal
盲注 The Blinds
发牌员 The dealer
钮扣 Button
小盲注 Small Blind
大盲注 Big Blind
窝牌 Hole Cards
悬牌 The Flop Cards
转牌 The Turn Card
河牌 The River Card
弃牌 Fold
看牌 Check
下注 Bet
跟注 Call
加注 Raise
再加注 Re-Raise
底池（彩池） Pot
全进 All-in