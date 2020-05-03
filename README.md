# System-eye 

Dual - Channel FFT Analyzer for macOS (beta). To test the app, download and unzip the .zip:

[>>> system-eye download page <<<](https://install.appcenter.ms/users/olegnaumenko/apps/system-eye/distribution_groups/external)

This app requires audio interface with minimum 2 separately connectable audio inputs to operate properly.

![system-eye screenshot](https://github.com/olegnaumenko/system-eye-osx-beta/blob/master/syseye-screenshot-small.png)

## Tips

System-eye is a dual - channel fft analyzer. It measures the Transfer Function of the system under test by means of comparison: it compares reference signal and signal produced by sending the reference through system under test, in frequency domain.

It was designed to be very simple and lightweight, supplying the core needs of experienced system engineer, without an overkill of well - known alternatives. 

It only supports one measurement channel pair at a time, and so far cannot do such advanced stuff as Live average. It doesn't support SPL/calibration whatsoever.

### Audio Input connection

Use external auido interface, input 1 - measurement mic, input 2 - reference signal. 
Select correct audio interface in Preferences;
Send the same reference signal to input 2 and to measured system (use some kind of split).
Use level indicator in the left bottom corner to make sure you get two distinct signals on reference and measurement channels.

### AutoDelay

Use AutioDelay button to turn on automatical delay detection between mic and reference. Without proper delay detection the measurement will be incorrect. Once you capture a trace of your measurement, Delta Delay reading becomes visible.

System-eye is equipped with pink noise generator that can be used as a reference signal.

### Captured traces

You can capture traces of Your measurement for future reference. Traces are stored in Trace Manager. You can open Trace manager using cmd+T keystroke, or using menu View -> Trace Manager. You can hide/show traces and delete them.

### Known issues:

- Flicker when resizing/maximizing the window
- Wrong sizing and line thickness when moving between screens with different content scale
- Plot positions are not saved on app exit

### Security concerns:

This buid has been notarized by Apple.

This beta app will collect anonymous telemetry info nessesary for futufe improvements.

### System requirements:

Minimum OS version is 10.10 Yosemite, but recommended minimum is 10.11 El Capitan. Compatible with macOS external audio interface is preferred.
