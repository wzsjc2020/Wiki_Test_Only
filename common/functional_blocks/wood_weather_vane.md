# 木风向标

Warning:此物品代码来自[Convenient Decor](  https://www.curseforge.com/minecraft/mc-mods/convenient-decor)模组，舒适空岛在原有代码的基础上进行了修改，遵循Apache 2.0 Licence

<div align=center><img src=../../resources/icon/wood_weather_vane-128px.png></div>

​     

| 添加此物品的原因 | Minecraft无法预知开始下雨和结束下雨的时间 |
| :--------------- | :----------------------------------------------------------- |
| 稀有度           | 常见                                                         |
| 命名空间         | comfysky:wood_weather_vane        |
| 添加版本         | 17.1.13                                                   |

​     

## 获取

工作台合成

​     

## 用途

预测开始或结束下雨的距离当前时间的时长

​     

## 交互

### 比较器输出

| 天气 | 红石信号强度对应         | 预测时间范围 | 红石信号强度 |
| ---- | ------------------------ | ------------ | ------------ |
| 晴天 | 距离开始下雨所需要的时长 | 0~15分钟     | 0~15（递增） |
| 雨天 | 距离停止下雨所需要的时长 | 0~15分钟     | 15~0（递减） |

注*：总体来说木风向标是一个很废物的东西，唯一作用是将下雨的信号转换成红石模电的信号。你也可以使用生电比如说狼甩尾巴或是阳光传感器感知天气来实现类似的功能

注*：作者认为[Convenient Decor](  https://www.curseforge.com/minecraft/mc-mods/convenient-decor)模组的算法会导致在下雨时风向标的摆动速度比不下雨时更慢不符合风向标在现实中的逻辑

**在舒适空岛中获取当前比较强输出强度的代码如下：**

这里的TimeUnit等于1200, 指代的是单位预测时间也就是1200tick(1分钟)，即1红石信号对应1分钟

```java
public static int getWeatherPredictionStrength(ServerWorld world, int timeUnit) {
    ServerWorldProperties properties = (ServerWorldProperties) world.getLevelProperties();
    if (world.isRaining() || properties.getClearWeatherTime() == 0) {
        return getStrengthFromRemainingTime(properties.getRainTime(), timeUnit, true);    //下雨
    }
    return getStrengthFromRemainingTime(properties.getClearWeatherTime(), timeUnit, false); //不下雨
}

/**
 * modified by comfysky
 */
public static int getStrengthFromRemainingTime(float remainingTime, int timeUnit, boolean isRaining) {
    int timeUnits = (int) (remainingTime / timeUnit);
    return MathHelper.clamp(isRaining ? timeUnits : 15 - timeUnits, 0, 15);
}
```

​     

### 风向标转动

当接近开始下雨时风向标的转动速度会增加，直到停止下雨，风向标的转动速度会逐渐减小

​     

## 数值表

| 常量             | 数据 | 数据类型 |
| :--------------- | ---- | -------- |
| @Debuggable      | true | boolean  |
| @broke instantly | true | boolean  |
| @TIME_UNIT       | 1200 | Integer  |

​     

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.20.1</td> <td width=120;>17.1.13</td> <td>加入了木风向标</td> </tr> </table>

​     

## 你知道吗

​     

## 参考

​     





