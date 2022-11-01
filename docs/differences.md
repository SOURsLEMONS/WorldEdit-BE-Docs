# 差异

由于这个插件仍在开发中，因此java原模组有很多功能是没有的;由于 Minecraft 的限制，某些功能根本无法实现。

## Commands

计划实现以下命令。

- /toggleplace
- /ascend
- /descend
- /ceil
- //sel
    - poly
    - ellipsoid
    - cyl
    - convex
- //chunk
- //size
- //curve
- //overlay
- //center
- //naturalize
- //deform
- //hollow
- /tool()
    - repl
    - deltree
    - lrbuild
    - floodfill
    - cycler
    - info
- /, (Super Pickaxe)
- /superpickaxe
    - single
    - area
    - recursive
- /brush 
    - butcher
    - clipboard
    - gravity
    - extinguish
    - raise
    - lower
    - set
    - deform
    - snow
- /listchunks
- /delchunks
- /remove
- //calculate

由于 API 限制，更改生物群系数据、使用图像或执行任何形式的任意文件操作的命令将更难实现，因此它们需要更长的时间才能成为插件的一个功能。


## 笔刷和工具

Items are not the only things you can bind to in the addon. Unlike the Java mod, you can also bind to blocks as well! Remember that once you bind a tool to a block, you can no longer place down that block until you unbind the tool/brush with either `;tool none` or `;brush none`.

## 选区

The only selection modes currently available are cuboid, extend and sphere. The other selection modes that you find in the planned command list will be implemented in the future.

One thing this has over the Java mod, is the ability to see selections, and not be limited to a specific version of Minecraft, or structure blocks. This can be toggled with `;drawsel`.

## 工具箱

Unlike the original mod, which was made for a game intended for keyboard only, this addon is made for all kinds of devices. The purpose of the kit, which you can get with `;kit`, is to be able to use WorldEdit's more common features more easily. See [Kit](usage/kit.md) for more info.
