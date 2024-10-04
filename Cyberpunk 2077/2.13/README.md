## Cyber Engine Tweaks

```
说明：控制台
时间：2024/9/13
网址：https://www.nexusmods.com/cyberpunk2077/mods/107
```

```shell
# 金钱
Game.AddToInventory("Items.money", 90000000)

# 义体词条随机性
ObserveBefore("RipperDocGameController", "StartCWUpgrade", function() Game.GetInventoryManager():IncrementCyberwareUpgradeSeed(2077) end)

```



```shell
# 义体容量(+6)
Game.AddToInventory("Items.CWCapacityPermaReward_Legendary",1)
```



```shell
# 技能芯片：猎头
Game.AddToInventory("Items.CoolSkill_Skillbook_Legendary",1)

# 技能芯片：黑客
Game.AddToInventory("Items.IntelligenceSkill_Skillbook_Legendary",1)

# 技能芯片：忍者
Game.AddToInventory("Items.ReflexesSkill_Skillbook_Legendary",1)

# 技能芯片：工程
Game.AddToInventory("Items.TechnicalAbilitySkill_Skillbook_Legendary",1)

# 技能芯片：独狼
Game.AddToInventory("Items.BodySkill_Skillbook_Legendary",1)

```



```shell

# 技能等级：猎头(35)
LvL = 35; ProfType = gamedataProficiencyType.CoolSkill; DS = PlayerDevelopmentSystem.GetInstance(Game.GetPlayer()):GetDevelopmentData(Game.GetPlayer()); DS:SetLevel(ProfType, LvL, telemetryLevelGainReason.Gameplay)

# 技能等级：黑客(35)
LvL = 35; ProfType = gamedataProficiencyType.IntelligenceSkill; DS = PlayerDevelopmentSystem.GetInstance(Game.GetPlayer()):GetDevelopmentData(Game.GetPlayer()); DS:SetLevel(ProfType, LvL, telemetryLevelGainReason.Gameplay)

# 技能等级：忍者(35)
LvL = 35; ProfType = gamedataProficiencyType.ReflexesSkill; DS = PlayerDevelopmentSystem.GetInstance(Game.GetPlayer()):GetDevelopmentData(Game.GetPlayer()); DS:SetLevel(ProfType, LvL, telemetryLevelGainReason.Gameplay)

# 技能等级：独狼(35)
LvL = 35; ProfType = gamedataProficiencyType.StrengthSkill; DS = PlayerDevelopmentSystem.GetInstance(Game.GetPlayer()):GetDevelopmentData(Game.GetPlayer()); DS:SetLevel(ProfType, LvL, telemetryLevelGainReason.Gameplay)

# 技能等级：工程(35)
LvL = 35; ProfType = gamedataProficiencyType.TechnicalAbilitySkill; DS = PlayerDevelopmentSystem.GetInstance(Game.GetPlayer()):GetDevelopmentData(Game.GetPlayer()); DS:SetLevel(ProfType, LvL, telemetryLevelGainReason.Gameplay)
```



## RED4ext

```
说明：脚本扩展器
时间：2024/9/12
网址：https://www.nexusmods.com/cyberpunk2077/mods/2380
```



## TweakXL

```
说明：TweakDB 修改加载器和脚本扩展
时间：2024/10/1
网址：https://www.nexusmods.com/cyberpunk2077/mods/4197
```



## Reset Attributes Always Available

```
说明：无限属性点重置
时间：2024/3/25
网址：https://www.nexusmods.com/cyberpunk2077/mods/9240
```



## Stock Market and News System

```
说明：股票市场
时间：2024/2/28
前置：CET
网址：https://www.nexusmods.com/cyberpunk2077/mods/6319
```



## Cyberware Max Out All Stat Rolls

```
说明：义体词条最大值
时间：2024/10/15
前置：CET、RED4ext、TweakXL
网址：https://www.nexusmods.com/cyberpunk2077/mods/10005
```



## Cyberware Stats Randomness Be Gone

```
说明：义体词条自定义
时间：2024/1/29
前置：CET、RED4ext、TweakXL
网址：https://www.nexusmods.com/cyberpunk2077/mods/12343
说明：在 "init.lua" 文件的 "DesiredModifiers" 部分添加词条，即可在义体升级页面显示。注意：最后一个元素尾部不需要 "," ，并且词条必须大于等于 3。
```

```
Modifiers.HealthRandom                                    生命值
Modifiers.HealthRegenRandom                               生命值回复
Modifiers.HealthRegenPercentRandom                        生命值回复加成
Modifiers.CritChanceRandom                                暴击率
Modifiers.CritDamageRandom                                暴击伤害
Modifiers.HealingItemsChargesRegenMultRandom              生命值物品补充速度
Modifiers.HealingItemsEffectPercentBonusRandom            生命值物品效果
Modifiers.MitigationChanceRandom                          半伤几率
Modifiers.MitigationStrengthRandom                        半伤强度
Modifiers.BonusQuickHackDamageRandom                      快速破解伤害
Modifiers.MeleeDamagePercentBonusRandom                   近战伤害
Modifiers.ReloadSpeedPercentBonusRandom                   装弹速度
```

