# Plant Monitor

An independent project to help decide when to check the moisture of one plant's growing medium. The first version will observe a real plant and give a cautious suggestion. It will not water automatically.

## Status

Initial definition. No sensor has been selected, and no physical prototype or calibration has been completed.

## Initial scope

- Collect readings that can be compared over time for the same plant.
- Suggest checking the growing medium only after several consistent readings indicate dryness under a calibrated rule.
- Show an unknown state when recent readings are missing or the sensor fails.
- Consider sending an alert to a central display later.

## Technology map

| Area | Current direction | Status |
| --- | --- | --- |
| Moisture sensing | Measure the growing medium for one specific plant; select and calibrate a probe after observing the real pot and medium. | Required capability; sensor technology open. |
| Local feedback | Show normal, check-medium, and unknown states. | Behavior proposed; physical interface open. |
| Connectivity | Local Wi-Fi may carry a later alert to the central display. | Candidate; not needed for the first local test. |
| Platform and power | Controller, firmware, power source, and enclosure. | Open pending placement and measurements. |
| Documentation and localization | Living English specifications; English and Spanish product text. Use Lingui if a JavaScript/TypeScript interface is built. | Language direction agreed; Spec Kit and Lingui not installed. |

## Documents

- [Pilot specification](specs/001-observe-growing-medium/spec.md).
- [Shared method and architecture](docs/method.md).
- [Program coordination in Notion](https://app.notion.com/p/416504754f0881afaaa6e4297e39c813).

## Next decisions

Test plant and pot; probe placement; sensor technology; power; calibration; reading frequency; threshold based on observed data; local alert channel.
