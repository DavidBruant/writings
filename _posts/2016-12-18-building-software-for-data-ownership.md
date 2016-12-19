---
published: false
---
## Data ownership

When entering data into a computer, everyone has an expectation that the computer will remember it. Either enough to transmit it to whoever we want to communicate it to or for personal archiving purposes. (let's ignore the [few cases](https://www.snapchat.com/) where one expects for the computer to forget the data purposefully).

* My data is mine
* Do not lose my data
* Let me share it and enable edition to others with fine granularity (both on the content and people levels)
* Let me create/edit anytime, whether I'm online or not


### My data is mine

I used your software to create data. It does not mean my data is yours. It doesn't mean I want you to read my data. Thank you for the tool, I'll keep the rest.

My data should be saved first and foremost on the device I created the data on.
* File system for desktop (database if useful)
* whatever file/storage API is available on mobile
* localStorage/IndexedDB in a browser

Then the data should be saved in a computer that is less likely to be lost/stolen/destroyed-by-mistake. Some people already have an online space to save data outside their own device:
* [Framadrop](https://framadrop.org/) (based on [lufi](https://framagit.org/luc/lufi) )
* Some [Remote Storage](https://remotestorage.io/)-compatible service
* Cozy?
* Dropbox
* Google Drive
* box.com

Allow the users to save their data in their places. Then and only then should you consider storing the data in your own servers 




### Do not lose my data

To the computer, data is data. To a human being, it took time before hitting the keyboard, clicking a mouse, voice inputing; before getting to a point where the data to be ready. Human beings, a single life, no time to waste; not on computer issues anyway.

Any software where data is entered in any way should save the data, so it's not lost. uh... automatically, in the background is meant. What is the deal with "save" buttons? And "restore" features? Just save the data and give it back to me when I'm back by default, without having me to do anything! Storage is cheap, the code is trivial to write, no excuse.

On my computer, use the file system. On the web use localStorage first, then send to a user-controlled data backup service or the server.

**Nobody should ever have to lose more than one minute of computer work.** 


### (read) Sharing

It's super rare that I type something in a computer with the sole intent of keeping it for myself. Any software should offer the possibility to share what's been created via URL.


### (edit) Sharing



## Review of a few softwares

* gmail.com VS email client
* prose.io
* 






Note to pierre Ozoux: what about a remoteStorage/Google Drive proxy?
User logs in to a remoteStorage Google app, user gets a remoteStorage URL. Data is effectively stored in Google Drive



