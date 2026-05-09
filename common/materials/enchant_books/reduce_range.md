# 范围减小

<div align=center><img src=../../../resources/icon/enchanted_book-128px.png></div>

​     

| 添加此物品的原因 | 模组前置              |
| :--------------- | :-------------------- |
| 稀有度           | 稀有                  |
| 命名空间         | comfysky:reduce_range |
| 添加版本         | 17.1.15               |

​     

## 获取

仅能从**古物研究学家**村民交易获取

无法从附魔台或宝藏获取

​     

## 用途

1.附魔在**挖掘铲（comfysky: digging_shovel）**上

当挖掘铲拥有此项附魔时，作用范围将减少，最低作用范围为1X1

​     

2.附魔在**半砖搬运器（comfysky: slab_transporter）**上

当半砖搬运器拥有此项附魔时，作用范围将减少，最低作用范围为1X1



作用范围计算公式：

```java
/*added since 17.1.15*/
public int getRangeByItemStack(ItemStack stack) {
    if (stack.hasEnchantments()) {
        int level = EnchantmentHelper.getLevel(ComfySkyEnchantments.REDUCE_RANGE, stack);
        return MathHelper.clamp(getRange() - level, 1, 5);
    }
    return getRange();
}
```

​     

## 交互

附魔可以堆叠

​     

## 数值表

| 常量       | 数据 | 数据类型 |
| :--------- | ---- | -------- |
| @MAX_LEVEL | 4    | int      |
| @MIN_LEVEL | 1    | int      |

​     

## 历史

<table border=1 style="width:100% ;height:100%"> <tr> <th align=center colspan=3>Java版</th> </tr> <tr> <td align=center rowspan=1 width=120; style="vertical-align:middle">1.20.1</td> <td width=120;>17.1.15</td> <td>加入了附魔范围减小</td> </tr> <tr></tr> </table>

​     

## 你知道吗

​     

## 参考

​     





