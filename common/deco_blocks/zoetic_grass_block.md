# 鲜活草地

<div align=center><img src=../../resources/icon/zoetic_grass_block-128px.png></div>

​     

| 添加此物品的原因 | Minecraft中花朵不可繁殖，补充空岛获得草方块的途径 |
| :--------------- | :------------------------------------------------ |
| 稀有度           | 常见                                              |
| 命名空间         | comfysky:zoetic_grass_block                       |
| 添加版本         | 17.0.13                                           |

​     

## 获取

1.手持**生长素**右键带有#zoetic_grass_can_spread方块标签的方块

```json
{
  "values": [
    "minecraft:dirt",
    "minecraft:grass_block",
    "minecraft:podzol",
    "minecraft:coarse_dirt",
    "minecraft:mycelium",
    "minecraft:rooted_dirt",
    "minecraft:moss_block",
    "minecraft:mud",
    "minecraft:muddy_mangrove_roots",
    "comfysky:suspicious_grass_block",
    "comfysky:suspicious_mud"
  ]
}
```

2.使用精准采集的工具采集掉落鲜活草地

3.使用非精准采集的工具掉落泥土

​     

## 用途

### 康威生命游戏

在鲜活草地上放置生命花模拟康威生命游戏

​     

### 还原草方块（1.20.1-17.1.15+）

当鲜活草地上方被方块阻挡时鲜活草地会在任意随机刻后还原成**草方块**

​     

## 交互

1.当游戏日（time of day）0~12000时，每20tick(1秒)进行一次康威生命游戏循环

2.鲜活草地会向四周带有#comfysky:zoetic_grass_can_spread标签的方块进行传播

3.是方块实体，无法被活塞推动

​     

## 数值表

| 常量        | 数据     | 数据类型 |
| :---------- | -------- | -------- |
| @TINT INDEX | 0x369E1D | RGB int  |

 <table border=1> <tr> <th align=left colspan=3> 标签 </th> </tr> <tr> <td align=center rowspan=2 width=120; style="vertical-align:middle"> 方块标签 </td> <td> #minecraft:mineable/shovel </td> </tr> <tr> <td> #dirt </td> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle"> NBT标签 </td> <td> #lastTickState </td> </tr> </table>

​    

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=3 width=120; style="vertical-align:middle">1.19.2</td> <td width=120;>17.0.13</td> <td>加入了鲜活草地</td> </tr> <tr> <td align=left rowspan=2 width=120; style="vertical-align:middle">17.0.14</td> <td>移除了合成配方</td> </tr> <tr> <td>现在鲜活草地由带有#zoetic_grass_can_spread方块标签的方块上右键使用生长素转换而来</td> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.19.4</td> <td width=120;>17.1.8</td> <td>现在鲜活草地上放置的植物会自动居中了</td> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.20.1</td> <td width=120;>17.1.15</td> <td>鲜活草地上方被方块阻挡时转化为草方块</td> </tr> </table>

​     

## 你知道吗

​     

## 参考

​     





