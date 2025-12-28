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

Import Instructions

⚠️ Important: Always back up your save file before making any changes.

1. **Preparation**

Create a manual backup of your No Man’s Sky save.

Open your save file using your preferred NMS save editor (e.g. NMSBaseJsonEditor).

2. **Importing Ship Data (Inventory / Class / Slots / Stats)**

Open
Spectre GOF2HD – ship data.json

Navigate to:

BaseContext
  └─ PlayerStateData
      └─ ShipOwnership[YY]


Replace one existing corvette slot with this data.

YY can be any value from 0 to 11 (12 ship slots total).

Important: This must be the same corvette you will modify in the construction step below.

3. **Importing Construction Data (Build / Parts / Layout)**

Open
Spectre GOF2HD – Construction Data.json

Navigate to:

BaseContext
  └─ PlayerStateData
      └─ PersistentPlayerBases[XX]


Locate the corvette base you want to replace.

⚠️ This section also contains planetary bases, so double-check before editing.

Replace the entire content of the selected corvette base with the Spectre construction data.

4.** Critical Data That MUST Be Preserved**

After pasting the Spectre construction JSON, restore the following values from your original corvette JSON.

4.1 Header values

(usually lines 15–16 or 16–17, depending on formatting)

      "UserData": XX,
      "LastUpdateTimestamp": zzzzzzzzzz,


➡️ These values must match your original corvette.

4.2 Footer / Ownership & Metadata block

At the end of the JSON file, the following section must also be preserved from your original corvette:

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
      "ScreenshotAt": [0.0, 0.0, 0.0],
      "ScreenshotPos": [0.0, 0.0, 0.0],
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


➡️ Do not copy these values from Spectre.
➡️ Always keep your original ownership, mode, and difficulty data.

5. Final Notes

Ship data and construction data are two separate datasets — both must reference the same corvette slot.

Incorrect ownership or base metadata will break the build or cause the corvette to disappear.

If something goes wrong: restore your backup and retry step by step.
## Notes
This build uses Atlas expedition components.
