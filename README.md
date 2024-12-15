# rtt
rTorrent rools

This repository contains small python scripts which helps me managing my rtorrent.

Tools so far:
* rtrssd: rTorrent RSS Downloader

## rtrssd:

About the tool in a nutshell:
* Parse a simple ini-style config file
* You can have several sections in there
* Process each section
* Check the first maxitems item in the rss feed (if maxitems is defined, otherwise all rss items will be checked),
* checks for every item, if that's loaded into your rtorrent
* If it's not:
  * download the torrent file
  * save it to your watchdir
  * wait for rtorrent to pick it up
  * than starts it

Example config file in the comment section of the code.
