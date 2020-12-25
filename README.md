# Voice / Mic Input Detection for Web with HTML & JS

This is a simple Javascript project to detect user voice input from mic for web apps. It can used to develop voice activated games, apps and others. Please note: it doesn't give you what user is saying but it give you if there is any kind of input (for example screaming) is coming or not.

## Demo

Test a live demo [Click Here](https://happy-newton-2ba6da.netlify.app/).



## Usage


var meter = createAudioMeter(audioContext,clipLevel,averaging,clipLag);

audioContext: the AudioContext youre using.
clipLevel: the level (0 to 1) that you would consider "clipping".  Defaults to 0.98.
averaging: how "smoothed" you would like the meter to be over time.  Should be between 0 and less than 1.  Defaults to 0.95.
clipLag: how long you would like the "clipping" indicator to show after clipping has occured, in milliseconds.  Defaults to 750ms.

meter.checkClipping();

returns true if the node has clipped in the last clipLag milliseconds.

meter.shutdown();

used to destroy the node (its important to disconnect and remove the event handler for any ScriptProcessor).



## Credits & Contributing

Developed from [Volume Meter](http://github.com/cwilso/volume-meter/).
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
