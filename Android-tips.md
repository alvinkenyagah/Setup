## Android tips
The following ADB command can be used to set a custom battery percent level to trigger battery save on Android 7.1:

```
adb shell dumpsys battery set level <battery_level>
```

Where `<battery_level>` is the desired battery level at which battery saver mode should be triggered. For example, to trigger battery saver mode at 50% battery, you would use the following command:

```
adb shell dumpsys battery set level 50
```

**Note:** You must have a rooted device in order to use this command.

To use this command, you will need to connect your device to your computer using a USB cable and enable ADB debugging. Once ADB debugging is enabled, you can open a terminal window on your computer and navigate to the directory where your ADB platform-tools are installed.

Then, you can use the above command to set the desired battery level for battery saver mode. For example, to trigger battery saver mode at 50% battery, you would use the following command:

```
adb shell dumpsys battery set level 50
```

Once you have set the desired battery level, you can disconnect your device from your computer. Battery saver mode will now be triggered at the specified battery level.

Please note that setting a custom battery level for battery saver mode may have an impact on your device's performance. It is important to monitor your device's battery life and performance after setting a custom battery level to ensure that it is working as expected.
