# DESCRIPTION

Modified version to work with edge.edx.org. 
Downloads subtitles from edge.edx.org but may not download them from edx.org.

Simple tool to download video lectures from edx.org.  It requires the
Python interpreter (> 2.6), youtube-dl, BeautifulSoup4 and it's
platform independent.  It should work fine in your Unix box, in
Windows or in Mac OS X.

# DEPENDENCIES

## youtube-dl

We use `youtube-dl` to download video lectures from Youtube, with the main
idea being that "we don't want to reinvent the wheel".  Make sure you have
`youtube-dl` installed in your system.  Also, since Youtube changes its
layout frequently, make sure that the version of `youtube-dl` that you have
installed is the latest. If in doubt, run `youtube-dl --update`.

You can find `youtube-dl` at <http://rg3.github.io/youtube-dl/download.html>.

## BeautifulSoup

Scrapping the web can be very silly task, but BeautifulSoup makes it
so easy :), it isn't included in the python standard library.  Make
sure you have BeautifulSoup installed.

You can install it with

    pip install beautifulsoup4

or

    easy_install beautifulsoup4.

For more info, see <http://www.crummy.com/software/BeautifulSoup/#Download>.

# Files

## edx-dl.py
Python implementation for edx-downloader

The original file was written by @shk3 in/for `python3` then updated
by @emadshaaban92 for python2, and migrated for versions superior to
2.6 by @iemejia.

# Quick Start

To use `edx-dl.py`, simply excute it, as in:

    python edx-dl.py

You will then be asked your username and password.

Your downloaded videos will be placed in a new Directory called
"Downloaded".  The script is very interactive, and if you have a issue
please tell us.

You can also excute it with arguments given: email and password,
as in:

    python edx-dl.py [-u user@user.com] [-p password]
