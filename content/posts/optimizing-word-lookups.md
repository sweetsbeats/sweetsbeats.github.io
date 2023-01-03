---
title: "Optimizing Word Lookups"
date: 2022-12-21T20:19:24-08:00
draft: false
tags: []
categories: [Japanese]
---

One of the more fun ways in which I've been immersing & mining recently has been reading manga. 
Most manga are still too hard to go alone on, but recently I've found myself reading yotsubato almost 
entirely without issue before bed or commuting to school on the bus. I consider this an important milestone 
in my learning; reaching a point where immersion converts from being an endeavour of practice to one of enjoyment is 
the end goal of learning any language. For manga that’s still a bit too hard for me, so I’ve created a decently 
efficient workflow for lookups and mining to make reading more fun.

The workflow makes use of mainly three tools: yomichan, sharex, and [manga-ocr](https://github.com/kha-white/manga-ocr). 
Manga-ocr is exactly what it sounds like: an OCR model trained on mostly manga and video games, 
and the workflow revolves around feeding it pictures of text.

We take a picture with ShareX, which is saved to a specific folder. 
This is best accomplished by creating a separate sharex workflow with a dedicated key combination, 
for reasons I’ll mention later (I use ctrl+alt+print_screen). 
Manga-ocr watches this folder and examines any new images saved to it, and places any extracted text into the clipboard. 
For the last leg of this process, Yomichan’s dedicated search page can be set to watch your clipboard for new text and perform a lookup.

In practice, it’s as simple as taking a picture of an unknown word or chunk of text using ShareX, 
and viewing the yomichan search page to see what it is. From there, you can use yomichan’s built in 
features to create an anki card using AnkiConnect, or just move on if you’re only doing lookups. 

As I mentioned earlier, using a separate sharex workflow that only saves to a folder has a unique advantage 
for card creation using yomichan, in that we can make cards with pictures of the manga panels in which we find words from. 
This is accomplished with the yomichan setting found under [Anki], which will insert whatever image is on the clipboard 
at the time of creation into your card. To do this ourselves, we first take a picture of the text with our sharex workflow, 
then screenshot the area we want using the default image region capture, and finally click the “add expression” button in yomichan.

All together, I’m quite happy with both the speed and quality of cards that come out, 
and I especially love getting to see the panel that I mined the word from. 
