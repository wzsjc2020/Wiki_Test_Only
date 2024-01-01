# 等距火把眼镜

<div align=center><img src=../../resources/icon/isometric_torch_spectacles-128px.png></div>

​     

| 添加此物品的原因 | 玩家更精准的放置火把                |
| :--------------- | :---------------------------------- |
| 稀有度           | 常见                                |
| 命名空间         | comfysky:isometric_torch_spectacles |
| 添加版本         | 17.1.12                             |

​     

## 获取

工作台合成

​     

## 用途

### 精准放置火把

每个玩家现在新增了一个全新的玩家属性：**火把放置距离**

当玩家装备等距火把眼镜，并手持火把，视线对准一个火把方块时，就可以在半径16格内以白色粒子效果显示下一根火把应该放置的位置（在大片平地上使用效果最佳）

​     

## 交互

1.佩戴在玩家头部装备栏时生效

2.手持等距火把眼镜 Shift+右键 增加玩家火把放置距离

3.当发射器激活时，可以穿戴在玩家的头部装备栏

​     

## 数值表

| 常量                           | 数据     | 数据类型 |
| :----------------------------- | -------- | -------- |
| @MAX_RAYCAST_DISTANCE          | 5        | int      |
| @MAX_PARTICLE_DISPLAY_DISTANCE | 16       | int      |
| @WHITE                         | 0xFFFFFF | Vector3f |

<table border=1> <tr> <th align=left colspan=3> 标签 </th> </tr> <tr> <td align=center rowspan=2 width=120; style="vertical-align:middle"> nbt </td> <td> TorchPlacementDistance </td> </tr> <tr> <td> BlockPos </td> </tr></table>

​     

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.20.1</td> <td width=120;>17.1.12</td> <td>加入了等距火把眼镜</td> </tr></table>

​     

## 你知道吗

​     

## 参考

​     





