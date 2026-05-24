# 铜静电球

<div align=center><img src=../../resources/icon/copper_electrostatic_ball-128px.png></div>

​     

| 添加此物品的原因 | Minecraft雷击平均时间约为10小时，雷电不能被存储，减少实体卡顿 |
| :--------------- | :----------------------------------------------------------- |
| 稀有度           | 常见                                                         |
| 命名空间         | comfysky:copper_electrostatic_ball |
| 添加版本         | 17.1.15                                                   |

​     

## 获取

工作台合成

​     

## 用途

当静电摩擦存储满（capacity >= 9999.0)，并且天空光等于15时，**方块上方产生一道雷电**

​     

## 交互

1.雨天不会产生静电摩擦

2.当方块中心 3x1x3 体积内有任意实体时，铜静电球每200tick累加一次静电摩擦，详细计算查看**铜静电球-数值表-静电收集**

3.使用比较器可以检测当前的容量

4.放置在任意方块上

5.**铜调试棒**右键铜静电球计算以当前产生静电摩擦的速率至存储满所需花费的时间

<img src="../../resources/screenshot/copper_electrostatic_ball.png" style="zoom:25%;" />

​     

## 数值表

| 常量              | 数据   | 数据类型 |
| :---------------- | ------ | -------- |
| @MAX_ESD_CAPACITY | 9999.0 | double   |

<table border=1> <tr> <th align=left colspan=3> 标签 </th> </tr> <tr> <td align=center rowspan=2 width=120; style="vertical-align:middle"> 方块标签 </td> <td> #minecraft:mineable/pickaxe </td> </tr> <tr> <td> #need_stone_tool </td> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle"> NBT标签 </td> <td> #capacity </td> </tr> </table>

​     

### 静电收集

<img src="../../resources/image/satatic_amount.png" style="zoom: 67%;" />

| 实体数量（x） | 静电量每200tick计算公式 |
| ------------- | ----------------------- |
| 0-100         | 0.00002*x^3             |
| 100-200       | -0.003*(x-200)^2+50     |
| 200-正无穷    | -(350/x)+51.75          |

计算过程： 

<img src="../../resources/image/calculate_electrostatic_amount.png" style="zoom: 67%;" />

常用参考数值：

| 实体数量(x) | 到达MAX所需时间（Minutes） |
| ----------- | -------------------------- |
| 100         | 83.3分钟                   |
| 200         | 33.3分钟                   |

​     

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=2 width=120; style="vertical-align:middle">1.19.2</td> <td width=120;>17.0.8</td> <td>加入了静电释放器</td> </tr> <tr> <td>17.0.9</td> <td>现在静电释放器放置具有方向性</td> </tr>  <tr> <td align=center rowspan=4 width=120; style="vertical-align:middle">1.20.1</td> <td align=left rowspan=4 width=120; style="vertical-align:middle">17.1.15</td> <td>移除了静电释放器</td> </tr> <tr> <td>加入了铜静电球</td> </tr> <tr> <td>更改了铜静电球的合成配方</td> </tr> <tr> <td>为了区分避雷针更改了铜静电球的方块模型</td> </tr> </table>

​     

## 你知道吗

1.铜静电球的原型来自于Minecraft中的避雷针

2.铜静电球在早期开发版中是有被雷击的方块状态的，你可以在assets\comfysky\textures\block中找到一个名叫electrostatic_discharge_rod_on.png的贴图，但是这个贴图从未使用过

3.铜静电球在早期开发版中的名字是电容

​     

## 参考

​     





