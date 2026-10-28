# Vodomerka-ESPHome

Modified ESPHome components for receiving Wireless M-Bus telegrams
using the CC1101 radio module and ESP32.

## Original project

Based on [hn/esphome-mbus](https://github.com/hn/esphome-mbus)
by Hajo Noerenberg.

The original copyright and license notices are retained.

## Modifications

- Modified the C1 Format B frame-length calculation in
  `components/mbus/wmbus_frame_codec.h`.
- Changed `return 1 + l_field + 2;` to `return 1 + l_field;`.
- Intended to correct CRC validation for Kamstrup flowIQ 2200 telegrams.

This modification is experimental and has not yet been
validated on the device.

## License

GNU General Public License version 3 (GPL-3.0).

See the LICENSE file for the complete license text.
