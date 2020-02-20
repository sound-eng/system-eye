# system-eye-osx-beta

To test the app, download and unzip the .zip:

[>>> system-eye download page <<<](https://install.appcenter.ms/users/olegnowmenco-gmail.com/apps/system-eye/distribution_groups/external)

Minimum OS version is 10.10 Yosemite. App requires external audio interface with minimum 2 audio inputs to make any sense.

![system-eye screenshot](https://github.com/olegnaumenko/system-eye-osx-beta/blob/master/syseye-screenshot-small.png)


## Tips

System-eye measures the Transfer Function of the system under test by means of comparison: it cpmpares reference signal and signal produced by sending the reference through system under test, in frequency domain.

It was designed to be very simple and lightweight, supplying the core needs if experienced system engineer without overkill of well - known alternatives. 

It only supports one measurement channel at a time, and so far cannot do such advanced stuff as Live average or Delta Delay. It doesn't support SPL/calibration whatsoever.

### Audio Input connection

Use external auido interface, input 1 - measurement mic, input 2 - reference signal. 
Select correct audio interface in Preferences;
Send the same reference signal to input 2 and to measured system (use some kind of split).

### AutoDelay

Use AutioDelay button to turn on automatical detection of the delay between mic and reference. Without proper delay the measurement will be incorrect.

System-eye is equipped with pink noise generator that can be used as a reference signal.

### Known issues:

- Flicker when resizing/maximizing the window
- Wrong sizing and line thickness when moving between screens with different content scale
- Plot positions are not saved on app exit

### Security concerns:

This buid has been notarized by Apple.

This beta app will collect anonymous telemetry info nessesary for futufe improvements.
