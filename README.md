# V3 (SX1262) bring-up evidence

Attachments for joyfulhouse/esphome-quietcool#49 (bring-up report) and #50 (wall-switch collision bug). This branch holds evidence only; it is not meant to be merged. The code and docs changes are in joyfulhouse/esphome-quietcool#51.

Board: Heltec WiFi LoRa 32 V3.2. ESPHome 2026.11.0. Component `v0.3.1`, plus a short re-check on main `b0d3fc5`. All logs were captured over the native API.

- `photos/`: board top with OLED test pattern (step 3b), board bottom, kit antenna.
- `logs/`: one log per guide step (file names match the report). Wi-Fi SSID, MACs and IPs are replaced with `<SSID>`, `<MAC>` and `<IP>`. The fan's sender ID `CB00E0C6` is left in.
  - `main-b0d3fc5/`: the re-check on main (cold boot, then query, commands and the switch collision).
  - `prior-run/`: an earlier session on the same board and firmware.
- `ha-history/`: Home Assistant history exports used for the soak (step 9): `Fan State Known` and `Heap Free`.
