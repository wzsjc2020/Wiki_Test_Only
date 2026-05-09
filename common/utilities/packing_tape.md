# 打包带

<div align=center><img src=../../resources/icon/packing_tape-128px.png></div>

​     

| 添加此物品的原因 | 李芒果空岛需要可以储存大量物品的容器，增加史莱姆农场的用途 |
| :--------------- | :--------------------------------------------------------- |
| 稀有度           | 常见                                                       |
| 命名空间         | comfysky:packing_tape                                      |
| 添加版本         | 17.0.4                                                     |

​     

## 获取

工作台合成

​     

## 用途

打包瓦楞纸箱（1.20.1-17.1.15+）

打包木桶（此特性已于1.20.1-17.1.15移除）

​     

## 交互

### 17.1.15+

Shift+右键瓦楞纸箱，如果瓦楞纸箱内没有带有#packing_black_list的物品，则打包成功，否则打包失败。打包完成后瓦楞纸箱会转化成打包过的瓦楞纸箱

#packing_black_list 物品标签

```json
{
  "values": [
    "comfysky:cardboard_box",
    "comfysky:packed_cardboard_box",
    "comfysky:packed_barrel",
    "minecraft:barrel",
    "minecraft:shulker_box",
    "minecraft:white_shulker_box",
    "minecraft:orange_shulker_box",
    "minecraft:magenta_shulker_box",
    "minecraft:light_blue_shulker_box",
    "minecraft:yellow_shulker_box",
    "minecraft:lime_shulker_box",
    "minecraft:pink_shulker_box",
    "minecraft:gray_shulker_box",
    "minecraft:light_gray_shulker_box",
    "minecraft:cyan_shulker_box",
    "minecraft:purple_shulker_box",
    "minecraft:blue_shulker_box",
    "minecraft:brown_shulker_box",
    "minecraft:green_shulker_box",
    "minecraft:red_shulker_box",
    "minecraft:black_shulker_box"
  ]
}
```

​     

### 17.1.15版本之前

Shift+右键木桶，如果木桶内没有带有#packing_black_list的物品，则打包成功，否则打包失败。打包完成后木桶会转化成打包过的木桶

​     

## 数值表

| 常量        | 数据 | 数据类型 |
| :---------- | ---- | -------- |
| @MAX_COUNT  | 1    | int      |
| @durability | 5    | int      |

​     

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.19.2</td> <td width=120;>17.0.4</td> <td>加入了打包带</td> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.20.1</td> <td width=120;>17.1.15</td> <td>现在无法对木桶(minecraft:barrel)使用打包带</td> </tr></table>

​     

## 你知道吗

打包带的原型来自于Storage Drawer模组

​     

## 参考

​     





