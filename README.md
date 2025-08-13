# General
```
- 012B260 = Current Mission index (Byte, starts at 0 then increments)

First level load or retry check(2 bytes are same on first load and then the same after every following load)
- 12B26C

[No Pain Sound Cooldown(Like Syphon Filter 1)]
Type = Gameshark
Activation = EndFrame
90135064 FFFFFFFF
```

# Weapon Ids
```
- 01 9MM
- 02 Silenced 9MM
- 03 45
- 04 M-16
- 05 Silenced HK-5
- 06 HK-5
- 07 PK-102
- 08 Shotgun
- 09 USAS-12
- 0A G18
- 0B BIZ-2
- 0C K3G4
- 0D H11
- 0E Silenced Sniper Rifle
- 0F Sniper Rifle(Not used)
- 10 Nightvision Sniper Rifle
- 11 Crossbow
- 12 Air Taser
- 13 Hand Taser
- 14 Knife
- 15 M-79
- 16 Grenades
- 17 Gas Grenades
- 18 C4
- 19 Transponder
- 1A ??
- 1B ??
```

# AI Stuff
```

AI Health is +28 Bytes after their weapon Id

;unlimited ammo, no fire cooldown, instant max Danger
;If level ticks not FFFFFFFF(paused or not in level)
;Activate conditional block
;if level index is not level 2(0x01) activate additional block that makes level 2 impossible otherwise
[Ridiculous AI Difficulty]
Type = Gameshark
Activation = EndFrame
A211ED30 FFFFFFFF
C611ED30 00000032
90133704 FFFFFFFF
901337F0 FFFFFFFF
901338DC FFFFFFFF
901339C8 FFFFFFFF
90133AB4 FFFFFFFF
80134BB2 000F
80134bf2 000F
80134C32 000F
80134C72 000F
80134CB2 000F
80134BB0 0000
80134bf0 0000
80134C30 0000
80134C70 0000
80134CB0 0000
80134B94 00000000
80134bd4 00000000
80134C14 00000000
80134C54 00000000
80134C94 00000000
00000000 FFFF
E112B260 0001
A211ED30 FFFFFFFF
80134BDE 2C
80134C9E 2C
80134C1E 2C
80134C5E 2C
80134B9E 2C
00000000 FFFF

[Tougher AI]
Type = Gameshark
Activation = EndFrame
Description = Remove AI's Pauses While Shooting + AI Max Danger
80134BB0 0000
80134bf0 0000
80134C30 0000
80134C70 0000
80134CB0 0000
90133704 FFFFFFFF
901337F0 FFFFFFFF
901338DC FFFFFFFF
901339C8 FFFFFFFF
90133AB4 FFFFFFFF

;Update 01/08/25 Fixed danger meter glitching on and off
;may have also made the AI miss less shots than previous method
[AI Instant MAX Danger]
Type = Gameshark
Activation = EndFrame
90133704 FFFFFFFF
901337F0 FFFFFFFF
901338DC FFFFFFFF
901339C8 FFFFFFFF
90133AB4 FFFFFFFF

[AI Unlimited Ammo]
Type = Gameshark
Activation = EndFrame
80134BB2 000F
80134bf2 000F
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
80134CB0 0000

[AI No Shoot Cooldown]
Type = Gameshark
Activation = EndFrame
80134B94 00000000
80134bd4 00000000
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

# AI Weapon Offsets
```
const AI_WEAPON_OFFSETS = {
    "Colorado Mountains":{
        "firstLoad": [
            "1AD724",
            "1AD8A0",
            "1AD8EC",
            "1AE0F0",
            "1AE188",
            "1AE220",
            "1AE1D4",
            "1AD984",
            "1AD640",
            "1AD68C",
            "1AD6D8",
            "1AD770",
            "1AD7BC",
            "1AD808",
            "1AD510",
            "1AD55C",
            "1AD5A8",
            "1AD5F4",
            "1ADA1C",//h11 before checkpoint
            "1AD9D0",//h11 before checkpoint
            "1AE13C",
            //missing H11 guys after checkpoint
        ],
        "retry": [
            "1AD200",
            "1AD37C",
            "1AD3C8",
            "1ADC18",
            "1ADCFC",
            "1ADCB0",
            "1ADC64",
            "1ADBCC",
            "1AD460",
            "1AD11C",
            "1AD168",
            "1AD1B4",
            "1AD24C",
            "1AD298",
            "1AD2E4",
            "1ACFEC",
            "1AD038",
            "1AD084",
            "1AD0D0",
            "1AD4F8", //h11 after checkpoint
            "1AD4AC", //h11 after checkpoint
            //"1AD4F8",//makes headshot h11 impossible to start
            //"1AD4AC"//makes headshot h11 impossible to start
            //find other 2 H11 addresses
        ]
    },
    "New York Sewers": {
        "firstLoad": [
            "1B434C",
            "1B4398",
            "1B43E4",
            "1B4300",
            "1B42B4",
            "1B1C1C",
            "1B1BD0",
            "1B1CB4",
            "1B1C68",
            "1B12E8",
            "1B1250",
            "1B129C",
            "1B1380",
            "1B13CC",
            "1B1334",
            "1B1464",
            "1B14B0",
            "1B1418",
            "1B14FC",
            "1B15E0",
            "1B162C",
            "1B1678",
            "1B16C4",
            "1B17F4",
            "1B1710",
            "1B175C",
            "1B17A8",
            "1B1840",
            "1B18D8",
            "1B1A54",
            "1B1AA0",
            "1B1A08",
            "1B1D98",
            "1B1DE4",
            "1B188C",
            "1B19BC",
            "1B1970",
            "1B1D4C",
            "1B1924",
        ],
        "retry": [ //1 ai with hk5 missed
            "1B4010",
            "1B40F4",
            "1B3FC4",
            "1B405C",
            "1B40A8",
            "1B18E0",
            "1B192C",
            "1B19C4",
            "1B1978",
            "19AE37",
            "1B0FAC",
            "1B0F60",
            "1B10DC",
            "1B1044",
            "1B1090",
            "1B1128",
            "1B1174",
            "1B11C0",
            "1B1258",
            "1B120C",
            "1B12F0",
            "1B133C",
            "1B1388",
            "1B13D4",
            "1B159C",
            "1B1420",
            "1B1504",
            "1B146C",
            "1B14B8",
            "1B1550",
            "1B15E8",
            "1B1764",
            "1B17B0",
            "1B1718",
            "1B1AA8",
            "1B1AF4",
            "1B16CC",
            "1B1680",
            "1B1A5C",
            "1B1634",
            "1B0FF8",
            "1B12A4",
        ]
    },"Finale": {
            "firstLoad": ["1B3064"],
            "retry": ["1B2FD0"]
        }
};
```