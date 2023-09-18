## Android tips

The following ADB command will trigger battery saver on at your specified set battery percentage:

```
adb shell settings put global low_power_trigger_level <percentage>
```

Replace `<percentage>` with the battery percentage at which you want battery saver to be triggered. For example, to trigger battery saver at 20%, you would use the following command:

```
adb shell settings put global low_power_trigger_level 20
```

You can verify that the battery saver trigger level has been set correctly by using the following command:

```
adb shell settings get global low_power_trigger_level
```

This will return the current battery saver trigger level.

**Note:** This command requires root access on your device.

Here is an example of how to use the command:

```
# Connect your device to your computer via USB.
# Enable ADB debugging on your device.
# Open a terminal window on your computer.
# Navigate to the directory where the ADB platform-tools are located.
# Run the following command to trigger battery saver at 20%:
adb shell settings put global low_power_trigger_level 20
# Verify that the battery saver trigger level has been set correctly:
adb shell settings get global low_power_trigger_level
```

This will return the following output:

```
20
```

This confirms that the battery saver trigger level has been set to 20%.
