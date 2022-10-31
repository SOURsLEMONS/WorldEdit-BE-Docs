# 配置

WorldEdit 的某些设置可以通过编辑与插件捆绑的配置文件来更改。此文件的位置取决于运行addon插件的平台，但相对于文件夹的路径是`com.mojang`文件夹下的`minecraftWorlds/(world folder)/behavior_packs/WorldEditB/scripts/config.js`

!!! Warning

    更新addon插件时，对此文件的任何更改都不会保留。您必须复制此文件，并在更新后将其放回原处以保留您的设置。

**Windows电脑**

``` txt
%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\(path to config)
```

**Android安卓**

``` txt
/storage/emulated/0/Android/data/com.mojang.minecraftpe/files/games/com.mojang/(path to config)
```
It's recommended that you use [CX File Explorer](https://play.google.com/store/apps/details?id=com.cxinventor.file.explorer) to access this path. You must also have Minecraft's storage mode set to External.

**iOS苹果**

``` txt
Minecraft/games/com.mojang/(path to config)
```

## Settings

| Setting | Default | Description |
| ------- | ------- | ----------- |
| DEBUG | false | 在内容日志中启用调试消息 |
| MAX_HISTORY_SIZE | 20 | 会话历史记录中可以记录多少个操作 |
| HISTORY_MODE | 2 (accurate) | 如何处理常规撤消和重做 |
| BRUSH_HISTORY_MODE | 1 (fast) | 如何处理画笔撤消和重做 |
| TICKS_TO_DELETE_SESSION | 12000 (10 mins) | 删除以前活跃用户的会话之前的时间 |
| PRINT_TO_ACTION_BAR | true | 是否使用项目将其消息打印到操作栏或聊天。 |
| COMMAND_PREFIX | ; | The character that every WorldEdit comman shoukd start with. |
| WAND_ITEM | minecraft:wooden_axe | The default item the selection wand is bound to from `;wand`. |
| NAV_WAND_ITEM | minecraft:ender_pearl | The default item the navigation wand is bound to from `;navwand`. |
| NAV_WAND_DISTANCE | 128 | How far the navigation wand, along with other tool, will trace for a block of interest. |
| MAX_BRUSH_RADIUS | 6 | 画笔允许的最大半径。 |
| DRAW_SELECTION | true | 默认情况下，玩家的选择是否可见 |
| DEFAULT_CHANGE_LIMIT | -1 | The default amount of blocks that can be "potentially" affected within a single operation |
| MAX_CHANGE_LIMIT | -1 | The absolute change limit that can be set from the `;limit` command; bypassed with `worldedit.limit.unlimited` permission |
| ASYNC_TIME_BUDGET | 200 | How long an async operation will run until giving Minecraft a chance to run; the higher the value, the faster the operation, but the slower Minecraft takes to run |
| FAST_MODE | false | Whether the addon should use simpler methods to run operations faster; this comes with the drawback of more limited capabilities |
