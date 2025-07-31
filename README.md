# General
```
012B260 = Current Mission index (Byte, starts at 0 then increments)

[No Pain Sound Cooldown(Like Syphon Filter 1)]
Type = Gameshark
Activation = EndFrame
90135064 FFFFFFFF
```

# AI Stuff
```

;128 value after player is out of sight or ignoring player
;0 if engage
;255 max danger/shooting
[AI Instant MAX Danger]
Type = Gameshark
Activation = EndFrame
8013370B FF
801337F7 FF
801338E3 FF
801339CF FF
80133ABB FF

[AI Unlimited Ammo]
Type = Gameshark
Activation = EndFrame
80134BB2 000F
80134bf2 000F
80134C32 000F
80134C72 000F
80134C32 000F
80134C72 000F
80134CB2 000F
80134CF2 000F

[AI No Shoot Delay]
Type = Gameshark
Activation = EndFrame
80134BB0 0000
80134bf0 0000
80134C30 0000
80134C70 0000
80134C30 0000
80134C70 0000
80134CB0 0000
80134CF0 0000

[AI No Shoot Cooldown]
Type = Gameshark
Activation = EndFrame
80134B94 00000000
80134bd4 00000000
80134C14 00000000
80134C54 00000000
80134C14 00000000
80134C54 00000000
80134C94 00000000
80134Cd4 00000000
```

# Weapon All Ammo Codes
```
[Infinite Ammo Silenced 9mm]
Type = Gameshark
Activation = EndFrame
8012A7F2 FFFF

[Infinite Ammo 9mm]
Type = Gameshark
Activation = EndFrame
8012A7F6 FFFF

[Infinite Ammo 45]
Type = Gameshark
Activation = EndFrame
8012A7FA FFFF

[Infinite Ammo M16]
Type = Gameshark
Activation = EndFrame
8012A7FE FFFF

[Infinite Ammo Silenced HK-5]
Type = Gameshark
Activation = EndFrame
8012A802 FFFF

[Infinite Ammo HK-5]
Type = Gameshark
Activation = EndFrame
8012A806 FFFF

[Infinite Ammo PK102]
Type = Gameshark
Activation = EndFrame
8012A80A FFFF

[Infinite Ammo Shotgun]
Type = Gameshark
Activation = EndFrame
8012A80E FFFF

[Infinite Ammo USA12]
Type = Gameshark
Activation = EndFrame
8012A812 FFFF

[Infinite Ammo G18]
Type = Gameshark
Activation = EndFrame
8012A816 FFFF

[Infinite Ammo BIZ-2]
Type = Gameshark
Activation = EndFrame
8012A81A FFFF

[Infinite Ammo K3G4]
Type = Gameshark
Activation = EndFrame
8012A81E FFFF

[Infinite Ammo H11]
Type = Gameshark
Activation = EndFrame
8012A822 FFFF

[Infinite Ammo Silenced Sniper Rifle]
Type = Gameshark
Activation = EndFrame
8012A826 FFFF

[Infinite Ammo Sniper Rifle]
Type = Gameshark
Activation = EndFrame
8012A82A FFFF

[Infinite Ammo Nightvision Sniper Rifle]
Type = Gameshark
Activation = EndFrame
8012A82E FFFF

[Infinite Ammo Crossbow]
Type = Gameshark
Activation = EndFrame
8012A832 FFFF

[Infinite Ammo M79]
Type = Gameshark
Activation = EndFrame
8012A842 FFFF

[Infinite Ammo Grenades]
Type = Gameshark
Activation = EndFrame
8012A846 FFFF

[Infinite Ammo Gas Grenades]
Type = Gameshark
Activation = EndFrame
8012A84A FFFF

[Infinite Ammo C4]
Type = Gameshark
Activation = EndFrame
8012A84E FFFF

[Infinite Ammo Tear-Gas Launcher]
Type = Gameshark
Activation = EndFrame
8012A85E FFFF
```


## C130 Wreck Site
```
//C130 wreck site AI weapon offsets
//76 bytes apart
01B0244
01B0290
01B02DC
01B0328
01B0374
01B03C0
01B04A4
01B040C
01B053C
01B0458
01B04A4
01B04F0
01B053C
01B0588
01B05D4
01B0620
01B066C
01B06B8
01B0704
01B0750
01B079C
01B07E8
01B0834
01B0880
01B08CC
01B0918
01B0964
01B09B0
01B09FC
01B0A48
```

# Finale
```
[Finale Give Chance M79]
Type = Gameshark
Activation = EndFrame
C01B37C8 0C44
801B3064 15
00000000 FFFF
C01B37C8 0668
801B2FD0 15
00000000 FFFF
```