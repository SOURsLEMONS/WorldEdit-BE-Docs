# 填充参数

创世神插件中的许多命令将填充参数作为它们的命令参数之一，填充参数决定了在世界中放置 _哪些哪种_ 方块

[目录]

## 填充参数模式

### 单块填充参数模式

这是最基本的常见 填充参数。使用这种类型只是按定义放置块。与 java mod 不同，您不能使用 数字ID 来指定方块。您可以改为通过其 字符串ID 和 可设置的方块属性(颜色种类) 来定义块。
语法如下：`命名空间:方块名[属性1=设定值,属性2=设定值,...]` 如果未指定方块属性，则将其保留为其默认值。 
原版方块可以省略原版命名空间 `minecraft` ，但是来自其他插件的方块是必需要加对应命名空间的。

指令例子↓

!!! Example

    `;set stone`
    
    将选区填充为普通石头。
    
    `;set wool[color=red]`
    
    将选区填充为红色羊毛。
    
    `;set stone_slab[stone_slab_type=brick,top_slot_bit=true]`
    
    将选区填充为石质上半砖

!!! Tip

    对方块使用 [「填充方块选取器」](/usage/kit#pattern_picker) 可以显示它字符串ID 和方块属性，这样您就可以知道字符串ID 和方块属性

!!! Note

   您还可以通过向字符串ID添加数据值来定义某些块变量。例如 `wool:1` 是橙色羊毛。这不能与方块属性一起使用。你可以在 我的世界Wiki 等地方找到方块具体数据值。

### 随机填充参数模式

可以设置一个随机填充参数，它可以包含多个单块填充参数，像这样(单块填充参数1,单块填充参数2,等等...)设置，逗号分隔每个单块填充参数。这将使各个单块填充参数均匀分布
想要某个 

可以制作一个模式来创建其他模式的混合。最简单的方法是制作一个逗号分隔的列表（）。这将使列表的元素均匀分布。要使一种模式比另一种模式更常见，可以向每个元素添加百分比 （）。数字越大意味着被置于手术中的机会就越大。这些数字加起来不必达到 100。

可以制作一个随机填充参数，创建其他填充的混合。最简单的方法是制作一个逗号分隔的列表（`填充1，填充2，等等..`）。这个列表的填充将均匀填充。要使一种填充比另一种填充更常见，可以向每个元素添加百分比（“percent%pattern，…”）。数字越大意味着接受手术的机会越大。这些数字加起来不必达到100。

It's possible to make a pattern that creates a mixture of other patterns. The simplest way is to just to make a comma separated list (`pattern1,pattern2,etc...`). This would make an even distribution of the list's elements. To make one pattern more common than an other, you can add percentages to each element (`percent%pattern,...`). A larger number means larger chance of being placed in an operation. The numbers don't have to add up to 100.

!!! Example

    `;set dirt,grass`
    
    This sets the region to half dirt, half grass.
    
    `;set 20%*wool,80%stone`
    
    This sets the region to 20% random wool, and 80% stone.

Notice in the last example, how block patterns aren't the only patterns you can use. There's more!

### Random State Pattern

Random state patterns create blocks with different random states. You make one by prefixing '\*' infront of a block ID. For example, `*log` would make logs of most types and in all directions. Most types because some logs use their own ID.

### Type/State Applying Pattern

Prefixing '^' to a block ID or block states allows you to change that aspect of blocks, and nothing more. Useful for when you want to change the type of a block without changing the orientation for instance.

!!! Example

    `;replace birch_stairs ^acacia_stairs`
    
    This turns birch stairs into acacia ones while keeping their orientation.
    
    `;replace wheat ^[growth=7]`
    
    This makes all wheat crops fully grown.
