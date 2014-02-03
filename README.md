Uses CirclePlayer version of jPlayer to integrate audio into a d3.js representation of a radio show clock.

CirclePlayer is a demo intended to showcase the jQuery HTML5 Media Library jPlayer
[https://github.com/happyworm/jPlayer](https://github.com/happyworm/jPlayer)

[Try the latest version.](http://happyworm.com/jPlayerLab/circleplayer/)

Uses HTML5 Audio, CSS3 Transforms (transform:rotate) hooks provided by : [https://github.com/lrbabe/jquery.rotate.js](https://github.com/happyworm/jPlayer)

A full browser fallback is planned, jPlayer provides the Flash HTML5 Audio fallback and the idea is to use a sprite map to display progress in non CSS3 compliant browsers. [http://modernizr.github.com/Modernizr/](http://modernizr.github.com/Modernizr/) could be used to check CSS3 transform:rotate compliance.

Possibilities exist to enhance the demo with [https://wiki.mozilla.org/Audio_Data_API](https://wiki.mozilla.org/Audio_Data_API) for supporting browsers.

Note the progress bar will not function correctly in Opera 11 due to a JIT compiler bug in the Opera browser : [http://twitter.com/dstorey/status/28108260418523137](http://twitter.com/dstorey/status/28108260418523137)

The demo's current look is heavily inspired by [http://forrst.com/posts/Untitled-CJz](http://forrst.com/posts/Untitled-CJz)

Thanks to [Jussi Kalliokoski](http://twitter.com/quinnirill) for contributing.

CirclePlayer is dual-licensed under the GPL and MIT licenses

# Running Timepiece

## Setup your machine
See [how to setup your mac to develop news applications like we do](http://blog.apps.npr.org/2013/06/06/how-to-setup-a-developers-environment.html) by the crew at NPR apps.

## Bootstrap the project
```
cd /path/to/timepice/repository/
mkvirtualenv timepiece
pip install -r requirements.txt
```

## Deploy to staging
```
workon timepiece
cd /path/to/timepiece/repository/
fab staging master deploy
```
*Warning*: This only works if we've set up an AWS IAM account for you.