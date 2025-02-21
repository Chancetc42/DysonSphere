# LaserClearing

![demo](https://raw.githubusercontent.com/starfi5h/LaserClearing/dev/img/demo.gif)  
Use mecha laser to auto-harvest trees and stones in range.  
The toggle button is right next to the battery bar.  
This mod is inspired by GreyHak's [DSP Drone Clearing](https://dsp.thunderstore.io/package/GreyHak/DSP_Drone_Clearing/).  
激光启用/关闭按钮在机甲能量条的右侧  

## Configuration
Run the game one time to generate `BepInEx\config\starfi5h.plugin.LaserClearing.cfg` file.  
配置文件(.cfg)需要先运行过游戏一次才会出现。修改后需重启游戏才会生效。    

```
## Settings file was created by plugin LaserClearing v1.0.4
## Plugin GUID: starfi5h.plugin.LaserClearing

[General]

## Enable LaserClearing when starting the game
## 进入游戏时启用激光
# Setting type: Boolean
# Default value: true
Enable = true

## Get drops from destroying trees and stones when enable laser
## 启用激光时,破坏树木/石头时会获取掉落物
# Setting type: Boolean
# Default value: true
EnableLoot = true

## Stop laser when there is not enough space in inventory
## 物品栏保留空位,当空间不足时停止激光
# Setting type: Int32
# Default value: 2
RequiredSpace = 2

[Laser]

## Maximum count of laser
## 激光最大数量
# Setting type: Int32
# Default value: 3
MaxCount = 3

## Maximum range of laser
## 激光最远距离
# Setting type: Single
# Default value: 40
Range = 40

## Time to mine an object (tick)
## 开采所需时间
# Setting type: Int32
# Default value: 90
MiningTick = 90

## Interval to check objects in range (laser cool-down time)
## 检查周期(激光冷却时间)
# Setting type: Int32
# Default value: 20
CheckIntervalTick = 20

## Power consumption per laser (kW)
## 激光耗能
# Setting type: Single
# Default value: 480
MiningPower = 480

[Other]

## Play sounds when trees and stones get clear by laser
## 激光清除树木/石头时播放音效
# Setting type: Boolean
# Default value: false
EnableDestructionSFX = false

[Target]

## Targets only objects with available drop
## 只清除有掉落物的植被
# Setting type: Boolean
# Default value: true
DropOnly = true

## Targets space capsule
## 清除飞行仓
# Setting type: Boolean
# Default value: false
SpaceCapsule = false
```
