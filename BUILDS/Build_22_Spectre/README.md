# Build 22 – SPECTRE

Manufacturer: Crimson Bureau of Advanced Architecture (CBAA)  
Class: Corvette  
Commission Type: Private order  
Status: Released  

## Description
Spectre is a stealth-oriented corvette commissioned for high-risk reconnaissance and precision strike operations.

## Included Files
- Spectre GOF2HD - Construction Data.json
- Spectre GOF2HD - ship data.json

## Import Instructions
1. Backup your save.
2. Import JSONs using your preferred NMS save editor.
3. Spectre GOF2HD - Construction Data.json - this data goes to BaseContext.PlayerStateData.PersistentPlayerBases[xx] - you need to find your Corvette build that you want to replace (this folder also contains your planetary bases - so be careful), and replace all code with the Spectre code - BUT BELOW VARIABLES AND THEIR VALUES MUST BE FROM YOUR ORIGINAL CORVETTE JSON:

      3.1 These two - lines 15 and 16, or 16 and 17:
            --------
            "UserData": XX,
            "LastUpdateTimestamp": zzzzzzzzzz,

   
      3.2 On the end of the JSON file:
             "Owner": {
                  "LID": "xxxxxxxxxx",
                  "UID": "xxxxxxxxxxxxxx",
                  "USN": "xxxxxxxxxxxxxx",
                  "PTK": "xxxxxxxxxxx",
                  "TS": xxxxxxxxxxxxxxxx
                },
                "Name": "xxxxxxxxxxxx",
                "BaseType": {
                  "PersistentBaseTypes": "PlayerShipBase"
                },
                "LastEditedById": "xxxxxxxxxxxxxxxxxxxxx",
                "LastEditedByUsername": "",
                "ScreenshotAt": [
                  0.0,
                  0.0,
                  0.0
                ],
                "ScreenshotPos": [
                  0.0,
                  0.0,
                  0.0
                ],
                "GameMode": {
                  "PresetGameMode": "xxxxxxxxxxxxxxx"
                },
                "Difficulty": {
                  "DifficultyPreset": {
                    "DifficultyPresetType": "xxxxxxxxxxxxxxxxxxx"
                  },
                  "PersistentBaseDifficultyFlags": 0
                },
                "PlatformToken": "",
                "IsReported": false,
                "IsFeatured": false,
                "AutoPowerSetting": {
                  "BaseAutoPowerSetting": "UseDefault"
                }
              }

      

5. Spectre GOF2HD - ship data.json goes to BaseContext.PlayerStateData.ShipOwnership[yy] - Y can be from 0 to 11 (12 slots), and you will be replacing the same corvette that you changed data in the previous point.
5.** Do not redistribute without credit.**

## Notes
This build uses Atlas expedition components.
