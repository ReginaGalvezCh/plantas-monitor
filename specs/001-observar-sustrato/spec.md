# Specification 001: Observe the Growing Medium

**Status:** proposal for validation.

## Purpose

Help decide when to check one specific plant without treating an isolated reading as proof that it needs watering.

## Expected behavior

1. The system records moisture readings for an identified plant and makes them comparable over time.
2. A suggestion to check the growing medium appears only after readings consistently meet the rule calibrated for that plant.
3. Old, missing, or inconsistent data produces an “unknown” state.
4. The suggestion can be dismissed or reset after checking the plant; the exact rule remains to be defined through testing.

## Pilot acceptance criteria

- Normal, “check growing medium,” and unknown states can be distinguished.
- A single anomalous reading does not trigger the suggestion.
- Sensor disconnection is not interpreted as dryness.
- The threshold is documented with observations from the test plant and is not presented as universal.

## Proposed first test

**Prerequisite:** choose and record a plant, pot, growing medium, use location, and probe. The test is not considered completed until physical measurements exist.

1. Mark an insertion position and depth so readings can be repeated without deliberately changing the geometry.
2. Record several consecutive readings before a normal watering, including time, raw value, manual observation of the growing medium, and probe position.
3. Record several readings after watering and through normal drying, keeping the position consistent. Note any changes to pot, growing medium, or location.
4. Compare variation among nearby readings with variation observed during drying. If they cannot be distinguished, revisit the sensor and method before proposing a rule.
5. Test an anomalous reading, a missing reading, and an old reading separately. They must produce a cautious state, never an instruction to water.
6. Document the data, observations, candidate rule, and exceptions. Set reading interval, data freshness, and the meaning of “consistent readings” from this evidence.

## Interpretation limit

The sensor observes one area of the growing medium; it does not diagnose the health of the whole plant. “Check growing medium” asks for a human check. “Water now” will not be inferred automatically from one isolated reading.

## Out of scope for now

Automatic watering, plant-health diagnosis, and synchronization with the central display.

## Open questions

Which plant and pot? Which probe technology will withstand the intended use? What reading interval and maximum data age are appropriate? How is the suggestion acknowledged?
