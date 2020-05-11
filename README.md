# biggy

A stand-alone web application that allows you to sync your data with Dropbox. 

# why the need for biggy (with a little bit of history)

A while ago I've found myself in a strange situation where I wasn't able to sync my old hard disk with Dropbox. The disk was   part of a RAID 1, consisting of two SATA disks (the other disk being corrupted and unreadable), which provided storage for my old midi tower desktop computer, which I had already sold and the only way for me to read the data from the disk was with a really crappy SATA to USB adapter. That was all fine until I've found out that my new shiny MacBook Pro wasn't able to speak to the crappy SATA to USB adapter. Luckily I also had two Raspberry Pis, who had no problem whatsoever to read the data from the disk. I thought that with that my problems were solved. That's when I had to find out that there is no ARM implementation of the Dropbox app. Of course I could've bought another not so crappy SATA to USB adapter, but then again I already hat a working hardware solution to my problem. I just needed a piece of software to somewhat automate the processs instead of using the Dropbox website for uploading a TB of data or curling my way through the API. 

***TL;DR***

I've looked around and wasn't able to find much. There were a bunch of Python solutions of course - like this one for instance - https://github.com/PapaCharlie/ARM-Dropbox, which didn't/don't work anymore. There were a couple of paid applications which came from companies that sold NAS devices. And of course there was/is also rclone. Now, rclone is really impressive. I've tested it and it would've solved my problem pretty neatly. Still, I wasn't content with the fact that there wasn't an API based solution with a nice clean GUI. 

So I've decided to give the Dropbox API a go and try to build a small plattform independent web application/REST client. The added value to this is that I would be able to play a bit with a real-life REST API and learn some stuff along the way. You might think of it more as a case study than an actual product.
