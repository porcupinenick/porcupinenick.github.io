---
layout: post
title: ClamAV - Antivirus for Everyone
subtitle: Catch those viruses...and keep them out!
cover-img: /assets/img/clamav.jpg
thumbnail-img: /assets/img/clamav.jpg
share-img: /assets/img/clamav.jpg
tags: [books, test]
---

Hey there, this is my first post! Recently, a friend of my introduced me to [ClamAV](https://www.clamav.net), an open-source anti-virus scanner for macOS, Windows and Linux. I've been using it for about 3 weeks now and...it's great! Here's a short snippet of how to install and/or run it:


## Installing ClamAV (I have not used ClamAV before):
1. Install ClamAV via Homebrew in the Terminal application. If you aren't sure if you have Homebrew or not, check out this post here.
```javascript
$ brew install clamav
```


2. Make the conf file
```javascript
$ mv /usr/local/etc/clamav/freshclam.conf.sample /usr/local/etc/clamav/freshclam.conf
```

3. Edit the conf file on line 8 (Example -> #Example) and save the changes
```javascript
#Example
```
