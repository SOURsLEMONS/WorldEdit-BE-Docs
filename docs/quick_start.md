# 快速入门

## 首先...

默认情况下，玩家不允许使用WorldEdit。只有那些标签标记为“worldedit”的人才能使用其功能。
要授予自己所有世界编辑权限，请在聊天栏输入 /tag @s add worldedit 
然后您应该会收到一条消息，指出您已获得在授予 WorldEdit 权限。
!!! Tip

    您还可以通过指定玩家的名称来授予其他玩家的世界编辑权限如果玩家的名称有空格，则需要用引号括起来。例如：@s/tag "玩家 名称" add worldedit

## 幻影移形(bushi)

!!! Notice

    此插件提供的命令使用分号作为前缀(;)而不是斜杠(/)。将来，Mojang可能会为Minecraft添加实际的自定义命令支持。
    
在复杂的地形间移动有时会很麻烦(很慢)。 幸运的是，这个插件带有所谓的传送器，请输入命令 ;navwand 获得一个末影珍珠 (直接物品栏拿一个也行)

获得此物品后，只需右键(长按)使用即可传送到您目光所至的位置。¹  
隔了一堵墙或天花板？潜行使用传送器直接穿过它！ ²  
卡在方块里？使用传送器会让你解开卡住！³  

!!! Tip

    如果您不想使用导航棒，也可以使用命令完成这些¹²³操作  ;jumpto ;thru ;unstuck

## 建立选区

与java版原模组相同,您可以使用选择器(小木斧)来标记世界中的区域以便进行各种操作，请拿起木斧，或输入命令。;wand 获得一个小木斧(直接物品栏拿一个也行)

创世神插件中的选区默认是方体形状的。为了形成一个选区,你需要标记立方体的两个对角:
第一点的选择方法是潜行状态下对目标点右键(长按)使用选择器;
第二点对目标点右键(长按)使用选择器，无需潜行(可在空中)
如果步骤正确，您应该会看到选区的粒子显示。

![Cuboid Selection](img/cuboid_selection.jpg)

如果没有块可供您标记角落，例如在高空中，  
您还可以使用 命令 分别标记第一个顶点 ;pos1 和第二个顶点 ;pos2 标记的点为玩家站立的位置(膝盖.绿玻璃)，不是脚下的方块。

![Position Placement](img/pos_placement.jpg)

## 快捷工具包

WorldEdit 中有许多我们可能常用的操作，例如撤消和复制选区，  
这些常见 WorldEdit 功能为了使此插件对移动和主机玩家更方便使用，它附带了一组快捷工具，输入命令。;kit 获得一个工具包

## 来亲自试试

选择适度大小的选择，并准备好您的快捷工具包。 
我们将尝试WorldEdit提供的一些功能。

1. 放一块石头，使用 [填充方块选取器](../usage/kit#pattern_picker) on it and use ["Fill Selection"](../usage/kit#selection_fill). A cuboid of stone should be made.
2. Use the Pattern Picker on the air (mobile players must hold the screen with it) and use "Fill Selection" again to clear the stone.
3. Place down sandstone and glass, use the Pattern pPicker on the sandstone, and sneak and use it on the glass to add to your pattern. Use "Fill Selection" and you should have a mix of sandstone and glass.
4. Take out the Mask Picker in your inventory and use it on the sandstone. Set a block of your choice as your pattern, and use "Fill Selection". All sandstone should now be replaced with that block.
5. Repeat your selection upwards by typing the command `;stack 4 up`.

If you want to you can undo everthing by using the undo item until you can't undo any further. You should also use `;mask` to clear the mask created previously.

## Playing with brushes

The kit also provides a way to make brushes.

1. Get a shovel of any type.
2. Place down cobblestone; you'll need it for the brush.
3. Use the ["WorldEdit Settings"](../usage/kit#config) item. A menu in your hotbar should appear including "Brush Settings". Select the item, then select the shovel to bind to. Make it a sphere brush of radius 3, and a cobblestone pattern. Confirm the settings and exit the menu.
4. Aim at the ground not near you and interact with the shovel (now brush) to place cobblestone spheres.
5. Make it so the brush only affects grass with `;mask grass` while holding the brush. Use the brush now to make a cobblestone path.
6. Disable the brush with `;br none` while holding said brush.

## What now?

You still have the rest of the docs you can look through. Go ahead and explore!
