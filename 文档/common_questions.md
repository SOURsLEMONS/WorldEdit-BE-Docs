# 常见问题

[目录]

## 如何使用这个插件？

文档充满了详尽的信息！作为初学者，最好从 [快速入门](quick_start.md) 页面开始 

## 它是否适用于主机平台?

从理论上讲，该插件应该可以在主机平台上运行，但尚未在这些主机上进行测试。Realm 可用于传输安装了插件的世界。

## 为什么插件对我不起作用？

插件无法正常工作的原因有四种可能。

1. 没有同时启用“假日创造者功能”和“测试版 API”。
2. 没有将行为包和资源包都应用到你的世界/存档。
3. 没有在正确的 Minecraft 版本上玩游戏。在撰写本文时，该插件支持 1.19 及更高版本。
4. 插件可能会为您损坏。没有已知的原因，但您可以尝试三件事。

    * 重新启动我的世界
    * 重新下载本插件
    * 重新安装我的世界

    您可以在 [此处](https://github.com/SIsilicon/WorldEdit-BE/issues) 报告该错误

## 我可以将WorldEdit与其他addon插件一起使用吗?

它应该与您世界中的任何其他addon插件兼容，但不能保证兼容性。

## How do I make coloured blocks, different types of wood, etc...?

How Minecraft works is that some blocks are just variations of a base block. Red wool for example is just a variation of the default white wool, and granite is just a variation of stone. To define these variations, you can use either data values (`wool:1` = orange wool), or block states (`stone_slab[stone_slab_type=brick]` = brick slabs). For more information on blocks in commands, go to [this docs page](usage/general/patterns.md).
 
## How do I remove selection particles?

That depends on the outcome you want.
- Use `;drawsel` to toggle the visiblity of the selection. The selection is still there, so you can still use your usual selection based commands.
- Use `;desel` to clear your selection (not the blocks inside. Use `;cut` for that). As soon as you start making your selection it will once again be highlighted with particles, unless you used `;drawsel` to disable it.

## How do I uninstall the addon from the world?

[See this section in the intallation page.](installation.md#uninstalling-from-a-world)

## Why does the message "Cannot modify unloaded chunks" show?

This usually is because the operation you're attempting, may also affect parts of your world that aren't "loaded"; loaded in the sense that things actually update in those chunks (grass growing, TNT exploding, redstone updating, etc...). If you can, perform your operation in smaller pieces. If not, make more chunks loaded by either increasing your Simulation Distance, or adding ticking areas where necessary.

## May I (use this on my server / showcase this)?

You are allowed to do so. Mind you that the addon is work in progress, so keep regular backups of your world.

## Are you affiliated with the original mod creators?

Nope! I developed this addon on my own.

## My question hasn't been answered here. Where else can I ask?

I have a [Discord](https://discord.gg/M5uAkr9WU2) server for this addon. You can go there, hangout, and ask away.
