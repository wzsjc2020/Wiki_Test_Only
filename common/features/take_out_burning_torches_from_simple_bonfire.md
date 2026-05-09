# 用木棍从简易篝火中取出点燃的火把

添加版本：v17.1.15

​     

在篝火点燃时，且拥有大于2000tick燃烧时长时，**主手手持木棍右键**简易篝火取出1根燃烧的火把，同时减少一定时长的燃烧时间

燃烧的火把燃烧时长计算公式：

```java
protected static final NormalDistribution DISTRIBUTION = new NormalDistribution(50, 15.6);

//理想燃烧时长取当前 (当前燃烧时长-1000,24000L)ticks, 火把燃烧最长时间是24000tick
long idealBurningTime = Math.min((burningTime - 1000), 24000L);
double zValue =DISTRIBUTION.percentile(world.getRandom().nextDouble());
//rationalized burnTime using normal distribution
long torchBurningTime = (long) ((long) idealBurningTime * (zValue / 100.0));
```

取出火把燃烧时长按mean=50, standard deviation =15.6的正态分布计算，玩家有80%的概率取出一个平均值在理想燃烧时长40%~70%的火把，最理想的情况下是取出一个无限接近于24000ticks 燃烧值的火把（约合20分钟现实时间），最糟糕的情况下是取出一个燃烧值为1000ticks燃烧值的火把（约合50秒现实时间）

​     

此特性无法通过配置文件关闭

​     

## 参考

漫漫长夜（The Long Dark）营火
