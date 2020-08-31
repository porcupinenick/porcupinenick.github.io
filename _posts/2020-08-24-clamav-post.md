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

* Note: I may release instructions about how to run ClamAV on a Windows and/or Linux machine.


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

## Running ClamAV (How do I use ClamAV after installing it):
1. Run 'freshclam' in the Terminal application
```javascript
$ freshclam
```


2. Make a text (.txt) file and list the files on your computer which you want to scan. Below is a sample of my text file (scan.txt)
```javascript
/Users/nicholaschen/Desktop
```


3. Navigate back to the Terminal application, locate the path to your scan file from Step 2, and type the following command, replacing the text between the quotes ('')
```javascript
$ sudo clamscan --file-list='REPLACE ME WITH THE PATH TO YOUR SCAN FILE, e.g. /Users/nicholaschen/Desktop/scan.txt'
```
