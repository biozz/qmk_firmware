# winry/winry25tc:via

This is a [VIA](https://www.caniusevia.com/) keymap, which is basically the same a default with the difference that `rules.mk` contains `VIA_ENABLE = yes`.

There is also `definition.json` file, which is used in [VIA App](https://usevia.app/). Make sure to enable **Show Design Tab** in the settings. Then upload the JSON file.

> Note: product and vendor ID are important and must the same as the ones in the `info.json` of the keyboard. Also, VIA uses those IDs without the leading `0x`.

You build and flash this keymap using following commands after setting up your QMK environment:

- `qmk compile -kb winry/winry25tc -km via`
- `qmk flash -kb winry/winry25tc -km via`

## Known issues

VIA might throw several warnings and errors related to `BACKLIGHT_CONFIG_GET_VALUE`, but that doesn't seem to impact any of its functionality.
