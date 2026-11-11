# Bluetooth Pairing Card (experimental)

An Omarchy Bluetooth panel clone that displays keyboard pairing codes in the card. Select an unpaired keyboard, then type the code shown on the keyboard and press Enter.

**Experimental:** Tested on a Logitech Craft to the point that the pairing code appeared. The agent currently rejects pairing methods requiring confirmation or entering a PIN on the computer; those devices may fail to pair using this panel. Error handling, cancellation, accessibility, translations and compatibility with other devices need further work. Use the stock panel or `bluetoothctl` if your device needs another pairing method.

Requires Omarchy's shell and BlueZ, Python 3, and PyGObject (Gio). The manifest retains the `fperez.bluetooth` identifier from the original personal clone, so installing it may conflict with an existing plugin of that name. Review the files and back up any existing plugin before installation.

To install after reviewing those limitations:

```bash
omarchy plugin add https://github.com/frank-blueview-ai/omarchy-bluetooth-pairing --enable
```

The panel and model are derived from [Omarchy](https://github.com/omacom/omarchy), copyright David Heinemeier Hansson and contributors, and distributed under the included MIT license.
