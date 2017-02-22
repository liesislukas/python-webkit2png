**webkit2png** 
==============

About
------
Python script that takes screenshots (browsershots) using webkit

##Installation
Ubuntu
------
- Add following packages: ``apt-get install python-qt4 libqt4-webkit xvfb``
- Install the flash plugin to screenshot Adobe Flash files: ``apt-get install flashplugin-installer``

Automated installation via ```pip```
-------------------------------------
- Install pip: ```apt-get install python-pip```
- Install webkit2png: ```pip install webkit2png```

Manual installation via Git
-----------------------------
- Install git: ``apt-get install git-core``
- Create directory: ``mkdir python-webkit2png``
- Clone the project: ``git clone https://github.com/adamn/python-webkit2png.git python-webkit2png``
- Install with: ``python python-webkit2png/setup.py install``

FreeBSD
-------
- install qt4 webkit: ```www/py-qt4-webkit, www/qt4-webkit, devel/py-qt4```
- install pip: ``devel/py-pip``
- install via: ``pip install webkit2png``

Usage
=====
- For help run: ``python scripts/webkit2png -h``

![Alt Text](http://24.media.tumblr.com/tumblr_m9trixXFHn1rxlmf0o1_400.gif)

```
Usage: webkit2png [options] <URL>

Creates a screenshot of a website using QtWebkit.This program comes with
ABSOLUTELY NO WARRANTY. This is free software, and you are welcome to
redistribute it under the terms of the GNU General Public License v2.

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  -x WIDTH HEIGHT, --xvfb=WIDTH HEIGHT
                        Start an 'xvfb' instance with the given desktop size.
  -g WIDTH HEIGHT, --geometry=WIDTH HEIGHT
                        Geometry of the virtual browser window (0 means
                        'autodetect') [default: (0, 0)].
  -o FILE, --output=FILE
                        Write output to FILE instead of STDOUT.
  -f FORMAT, --format=FORMAT
                        Output image format [default: png]
  --scale=WIDTH HEIGHT  Scale the image to this size
  --aspect-ratio=RATIO  One of 'ignore', 'keep', 'crop' or 'expand' [default:
                        none]
  -F FEATURE, --feature=FEATURE
                        Enable additional Webkit features ('javascript',
                        'plugins')
  -c COOKIE, --cookie=COOKIE
                        Add this cookie. Use multiple times for more cookies.
                        Specification is value of a Set-Cookie HTTP response
                        header.
  -w SECONDS, --wait=SECONDS
                        Time to wait after loading before the screenshot is
                        taken [default: 0]
  -t SECONDS, --timeout=SECONDS
                        Time before the request will be canceled [default: 0]
  -W, --window          Grab whole window instead of frame (may be required
                        for plugins)
  -T, --transparent     Render output on a transparent background (Be sure to
                        have a transparent background defined in the html)
  --style=STYLE         Change the Qt look and feel to STYLE (e.G. 'windows').
  --encoded-url         Treat URL as url-encoded
  -d DISPLAY, --display=DISPLAY
                        Connect to X server at DISPLAY.
  --debug               Show debugging information.
  --log=LOGFILE         Select the log output file
```
