# Plant Monitor

An independent project to help decide when to check the moisture of one plant's growing medium. The first version will observe a real plant and give a cautious suggestion. It will not water automatically.

## Status

Initial definition. No sensor has been selected, and no physical prototype or calibration has been completed.

## Initial scope

- Collect readings that can be compared over time for the same plant.
- Suggest checking the growing medium only after several consistent readings indicate dryness under a calibrated rule.
- Show an unknown state when recent readings are missing or the sensor fails.
- Consider sending an alert to a central display later.

## Documents

- [Pilot specification](specs/001-observar-sustrato/spec.md).
- [Shared method and architecture](docs/metodologia.md).
- [Program coordination in Notion](https://app.notion.com/p/416504754f0881afaaa6e4297e39c813).

## Next decisions

Test plant and pot; probe placement; sensor technology; power; calibration; reading frequency; threshold based on observed data; local alert channel.
