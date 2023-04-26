# 打包过的木桶

<div align=center><img src=../../resources/icon/packed_barrel-128px.png></div>

​     

| 添加此物品的原因 | 李芒果空岛需要可以储存大量物品的容器 |
| :--------------- | :----------------------------------- |
| 稀有度           | 常见                                 |
| 命名空间         | comfysky:packed_barrel               |
| 添加版本         | 17.0.4                               |

​     

## 获取

生存模式无法获取该物品

​     

## 用途

1.破坏后打包过的木桶内的物品以NBT的形式保存在物品组中

​     

## 交互

1.打包带shift+右键木桶在打包成功后转化为打包过的木桶，打包时木桶物品列表中带有#barrel_packing_blacklist物品标签的物品会导致打包失败

2.带有#barrel_packing_blacklist物品标签的物品无法通过漏斗传入此容器

​     

## 数值表

| 常量                    | 数据 | 数据类型 |
| :---------------------- | ---- | -------- |
| @MAX_BARREL_DISPLAY_INV | 4    | int      |

<table border=1> <tr> <th align=left colspan=3> 标签 </th> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle"> 方块标签 </td> <td> #minecraft:mineable/axe </td> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle"> 物品标签 </td> <td> #barrel_packing_blacklist </td> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle"> NBT标签 </td> <td> #Items </td> </tr> </table>

​     

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=5 width=120; style="vertical-align:middle">1.19.2</td> <td width=120;>17.0.4</td> <td>加入了打包过的木桶</td> </tr> <tr> <td width=120;>17.0.5</td> <td>修复了木桶带nbt标签时tooltip不显示前4个物品的BUG</td> </tr> </tr> <tr> <td width=120;>17.0.6</td> <td>现在木桶中带有barrel_packing_black_list标签的物品时无法打包</td> </tr> </tr> <tr> <td width=120;>17.0.7</td> <td>修复了打包后带有barrel_packing_black_list标签的物品可以通过漏斗传入的BUG</td> </tr> </tr> <tr> <td width=120;>17.1.0</td> <td>修复了状态发生改变时未删除BlockEnitity从而导致物品复制的高危BUG</td> </tr> </table>

​     

## 你知道吗

1.当玩家试图尝试打包含有barrel_packing_black_list标签物品的木桶时会弹出红色警告 **禁止套娃**

​     

## 参考

​     





