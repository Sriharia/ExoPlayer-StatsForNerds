Demo app to showcase Google ExoPlayer customisations like player stats extractions, Improved buffering. 

More information on ExoPlayer documentation can be found [here][]

[here]: http://google.github.io/ExoPlayer/

### Developed by
[Srihari Yachamaneni](https://github.com/Sriharia) ([@srihari_y](https://twitter.com/srihari_y))

# Features #
## Stats for Nerds ##
This demo app depicts ExoPlayer internal stats in dynamic charts using [MPAndroidChart][] library.
These stats include:
<ul>
<li>Connection Speed</li>
<li>Buffer Size in Seconds</li>
<li>Network Activity</li>
<li>Dropped Frames</li>
</ul>

![Sample](screens/charts.jpg?raw=true "Demo app stats")

This is achieved by injecting a listener to a [Customised][] version of [LoadControl][] component of ExoPlayer

[MPAndroidChart]: https://github.com/PhilJay/MPAndroidChart
[Customised]: https://github.com/google/ExoPlayer/blob/d979469659861f7fe1d39d153b90bdff1ab479cc/library/core/src/main/java/com/google/android/exoplayer2/DefaultLoadControl.java
[LoadControl]: https://github.com/google/ExoPlayer/blob/d979469659861f7fe1d39d153b90bdff1ab479cc/library/core/src/main/java/com/google/android/exoplayer2/DefaultLoadControl.java

## Improved Buffering ##
This demo also helps you to find a way to change max buffer time by applying "drip-feeding" method.
This is achieved by changing certain parameters in custom LoadControl component of ExoPlayer

Check [CustomLoadControl][] class for more info on how buffer improvements are handled.
 
 [CustomLoadControl]: https://github.com/google/ExoPlayer/blob/d979469659861f7fe1d39d153b90bdff1ab479cc/library/core/src/main/java/com/google/android/exoplayer2/DefaultLoadControl.java