---
published: false
---
## Data ownership

It can be a [blog post](https://github.com/DavidBruant/writings/blob/gh-pages/_posts/2016-12-18-building-software-for-data-ownership.md), a poem, conversations with loved ones, your favorite places to get [tea](http://verdenero.fr/) (they have wonderful coffee i understand, by I don't drink any), drafts of a song, [a funny video](https://www.youtube.com/watch?v=vIV6MU4Yqek), filling some spreadsheets for the viability of a project, or just regular accounting; heck! the latest code you've written or maybe data about your tastes or professional connections.
When entering data into a computer, everyone has an expectation that the computer will remember it. Either enough to transmit it to whoever we want to communicate it to or for personal archiving purposes. (let's ignore the [few cases](https://whispersystems.org/blog/disappearing-messages/) where one expects for the computer to forget the data purposefully).

For all practical purposes, creation of data is necessarily mediated through software. This article lays out some principle about how i believe software should behave with regards to the data i've created.

It can be sumarized as follows:
* My data is mine
* Do not lose my data
* Let me share it and enable edition to others with fine granularity (both on the content and people levels)
* Let me create/edit anytime, whether I'm online or not


### My data is mine

I used your software to create data. It does not mean my data is yours. It doesn't mean I want you to read my data. Thank you for the tool, I'll keep the rest.

Until i've given you explicit consent, you don't copy my data to your servers, you don't analyze it, you don't target ads at my face.

Terms of Services are good when you're trying to protect yourself from legal consequences, but [they're a lie](https://tosdr.org/). You know it, i know it, everyone does. They're nowhere near being enough from a moral standpoint to be understood as consent. More is expected. I don't care it owning my data does not fit in your business plan.

For the purpose of finding my data on different devices, it's fine to use a server, but it should be some data storage location that i own. Some people already have an online space to save data outside their own device like Google Drive or Dropbox.


### Do not lose my data

YOLO. I mean... seriously. Time is precious!

To the computer, data is data. To a human being, it took time before hitting the keyboard, clicking a mouse, voice inputing; before getting to a point where the data to be ready. Human beings, a single life, no time to waste; not on computer issues anyway.

Any software where data is entered in any way should save the data, so it's not lost. This should happen automatically, in the background. What is the deal with "save" buttons? And "restore" features? Just save the data and give it back to me when I'm back by default, without having me to do anything! Storage is cheap, the code is trivial to write, no excuse.

On my computer, use the file system. On the web use localStorage first, then send to a user-controlled data backup service or the server.

**Nobody should ever have to lose more than one minute of computer work.** 


### (read) Sharing

It's rare that I create data in a computer with the sole intent of keeping it for myself. Any software should offer the possibility to share what's been created via URL.


### (edit) Sharing



## Review of a few softwares

* gmail.com VS email client
* prose.io
* 



My data should be saved first and foremost on the device I created the data on.
* File system for desktop (database if useful)
* whatever file/storage API is available on mobile
* localStorage/IndexedDB in a browser

Then the data should be saved in a computer that is less likely to be lost/stolen/destroyed-by-mistake. Some people already have an online space to save data outside their own device:
* [Framadrop](https://framadrop.org/) (based on [lufi](https://framagit.org/luc/lufi) )
* Some [Remote Storage](https://remotestorage.io/)-compatible service
* Maybe something based on [Tahoe fs](https://tahoe-lafs.org/trac/tahoe-lafs)
* Cozy?
* Dropbox
* Google Drive
* box.com

Allow the users to save their data in their places. Then and only then should you consider storing the data in your own servers 






Note to pierre Ozoux: what about a remoteStorage/Google Drive proxy?
User logs in to a remoteStorage Google app, user gets a remoteStorage URL. Data is effectively stored in Google Drive
