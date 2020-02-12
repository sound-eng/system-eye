# system-eye-osx-beta

To test the app, download and unzip the .zip:

[https://github.com/olegnaumenko/system-eye-osx-beta/blob/master/system-eye-1-0-notarized-beta.zip](https://github.com/olegnaumenko/system-eye-osx-beta/blob/master/system-eye-1-0-notarized-beta.zip)

Minimum OS version is 10.10 Yosemite. App requires external audio interface with minimum 2 audio inputs to make any sense.

![system-eye screenshot](https://github.com/olegnaumenko/system-eye-osx-beta/blob/master/syseye-screenshot.png)


Tips:

System-eye measures the Transfer Function of the system under test by means of comparison of reference signal and signal produced by sending the reference through system under test.

Audio Input connection:

Use external auido interface, input 1 - measurement mic, input 2 - reference signal. 
Select correct audio interface in Preferences;
Send the same reference signal to input 2 and to measured system (use some kind of split).

Use AutioDelay button to turn on automatical detection of the delay between mic and reference. without proper delay the measurement will be incorrect.

System-eye is equipped with pink noise generator that can be used af reference signal.

Known issues:

- In preferences, channle swapping controls don't work
- In preferences, noise generator volume doesn't work
- Generator sometimes won't start. requires re - selecting the output audio card
- Flicker whe resizing/maximizing the window
- wrong sizing and line widths when moving between screens with different content scale
- plot positions are not saved on app exit
