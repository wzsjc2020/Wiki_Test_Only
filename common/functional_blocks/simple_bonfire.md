# 简易篝火

<div align=center><img src=../../resources/icon/simple_bonfire-128px.png></div>

​     

| 添加此物品的原因 | 减少GUI使用，烧炼碎矿，取出火把，模组前置 |
| :--------------- | :---------------------------------------- |
| 稀有度           | 常见                                      |
| 命名空间         | comfysky:simple_bonfire                   |
| 添加版本         | 17.1.8                                    |

​     

## 获取

工作台合成

​     

## 用途

### 模组前置

在李芒果空岛前期，可以通过简易篝火熔炼碎矿从而获取金属粒，从而增加了一种除打僵尸掉铁锭外额外的一种获取铁锭的方式

当玩家放置简易篝火后，篝火会持续燃烧200Ticks（10秒）如果在这段时间内未添加燃料则篝火会在200Ticks 后熄灭

注意：李芒果空岛前期无法获取打火石，请格外珍惜火源，不要让其熄灭，否则使用非精准采集的工具破坏时会损失大约72%原料

​     

### 取出火把

在篝火点燃时，且拥有大于100tick燃烧时长时取出1根火把，同时减少100tick的燃烧时长

​     

### 烧炼物品

<img src="../../resources/screenshot/simple_bonfire.png" style="zoom:25%;" />

简易篝火具有两个烧炼物品槽，位于简易篝火体积最大的两块石头上

安装ERI后鼠标指针悬浮于该物品上，可以按U键可查看所有加入的简易篝火配方

当物品烧炼完成后不会像原版篝火那样直接掉落

注意：当篝火熄灭时，未完成烧炼的物品进度将重置

​     

## 交互

1.主手手持木棍（minecraft:stick）右键点击篝火，减少篝火100燃烧值，取出一根火把

2.主手手持火焰弹或打火石右键点击篝火，点燃篝火

3.手持铲子右键点击篝火，熄灭篝火

4.手持任意燃烧值不为0的物品右键篝火，增加对应燃烧时间，最大燃烧时间为5000ticks

5.手持任意物品右键烧炼槽位，GUI会显示放入的物品，并尝试烧炼，再次右键烧炼槽位取出物品

6.使用精准采集附魔的物品会掉落一个简易篝火，否则则会掉落18至27个碎石

​     

## 数值表

| 常量                 | 数据       | 数据类型 |
| :------------------- | ---------- | -------- |
| initial burning time | 200 ticks  | integer  |
| MAX_BURNING_TIME     | 5000 ticks | integer  |
| inventory size       | 2          | integer  |

<table border=1> <tr> <th align=left colspan=3> 标签 </th> </tr> <tr> <td align=center rowspan=4 width=120; style="vertical-align:middle"> 方块标签 </td> <td> #minecraft:mineable/axe </td> </tr> </table>     

​     

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.19.4</td> <td width=120;>17.1.8</td> <td>加入了简易篝火</td> </tr> </table>

​     

## 你知道吗

1.简易篝火使用的配方类型是壁炉（RecipeType.FIREPLACE），这是作者故意为之

这个壁炉中大部分代码是由乡野装饰壁炉被弃用的代码复制而来

2.简易篝火的原型源自于漫漫长夜（The Long Dark）中的营火

​     

## 参考

​     





