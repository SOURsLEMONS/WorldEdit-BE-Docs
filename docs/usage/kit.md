# 工具包

由于 创世神基岩版 是为不同的设备制作的，因此作者创建这个快捷工具包是为了使其更容易在任何设备上使用;无论是键盘、触摸屏还是手柄。它快捷使用创世神的常用操作;例如撤消，重做，复制和粘贴。

## Main items

输入命令`;kit`,您将获得以下快捷工具:

* <a name="selection_wand"></a>**选择器 ![](../img/icons/wood_axe.png):** 用来设置选区顶点 您可以使用命令  `;desel` 删除您的选区 . 请参阅 [选区](regions/selection.md).
* <a name="selection_fill"></a>**填充选区 ![](../img/icons/selection_fill.png):** 用填充方块选取器选取的方块填充选区。
* <a name="pattern_picker"></a>**填充方块选取器 ![](../img/icons/eyedropper.png):** Select blocks to use in a pattern. Sneaking will add blocks to the pattern. The pattern is used by various tools in the kit such as "Fill Selection".
* <a name="copy"></a>**复制 ![](../img/icons/copy.png):** 将选区复制到剪贴板。
* <a name="cut"></a>**剪切 ![](../img/icons/cut.png):** 将选区复制到剪贴板，然后用空气填充选区。
* <a name="paste"></a>**粘贴 ![](../img/icons/paste.png):** 将剪贴板中的任何内容粘贴到世界。粘贴的位置相对于上次复制/剪切时的所选内容。请参阅 [剪切板](clipboard.md).
* <a name="undo"></a>**撤销 ![](../img/icons/undo.png):** 撤消您之前影响世界的操作。（不撤销选区） 请参阅 [历史记录](general/history.md).
* <a name="redo"></a>**还原 ![](../img/icons/redo.png):** 重做你之前影响世界的行动。 请参阅 [历史记录](general/history.md).
* <a name="config"></a>**创世神设置 ![](../img/icons/config.png):** Enter a hotbar menu to change and setup some things about WorldEdit and the kit.
* <a name="flip"></a>**翻转 ![](../img/icons/flip.png):** 相对于玩家面向方向从左向右翻转所选内容。潜行使用会让它在选区中心翻转。
* <a name="rotate"></a>**旋转 ![](../img/icons/rotate_cw.png) ![](../img/icons/rotate_ccw.png):** 相对于玩家面向方向旋转所选内容。潜行使用会使它绕选区中心旋转。
* <a name="mask_picker"></a>**取代方块选取器 ![](../img/icons/maskdropper.png):** Select blocks to use in the global mask. Like the Pattern Picker, sneaking will add blocks to the mask. This affects "Fill Selection", and the brushes. To clear it, use the command `;gmask`.
* <a name="draw_line"></a>**填充选区对角线 ![](../img/icons/draw_line.png):**  用填充方块选取器选取的方块填充一条直线在选区两点
* <a name="selection_wall"></a>**填充选区的侧面 ![](../img/icons/selection_wall.png):** 用填充方块选取器选取的方块填充选区的侧面（前后左右4个面）。
* <a name="selection_outline"></a>**填充选区表面 ![](../img/icons/selection_outline.png):** 用填充方块选取器选取的方块填充选区的表面（前后左右上下6个面）。
* <a name="spawn_glass"></a>**在脚下生成玻璃方块 ![](../img/icons/spawn_glass.png):** 在你站立的地方填充一个玻璃块。当需要在半空中设置选区顶点标记时很有用。
* 
## 创世神设置

使用“创世神设置” 在物品栏中打开一个菜单。不用担心！之前物品栏中的任何物品都会在您退出菜单后还原。目前有三个按钮？。

* **在剪贴板中包含空气 ![](../img/icons/include_air.png):** 选择是否将空气复制到剪贴板。否则，粘贴时不会保留空气
* **在剪贴板中包含实体 ![](../img/icons/include_entities.png):** 选择是否将实体复制到剪贴板。禁用后剪切时，选区中的实体将被删除。
* **工具设置 ![](../img/icons/tool_config.png):** 创建和管理工具。
* **笔刷设置 ![](../img/icons/brush_config.png):** 创建和管理笔刷。使用它之前，建议先将填充方块以及取代方块准备好，更好的设置笔刷
