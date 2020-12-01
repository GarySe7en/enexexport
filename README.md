# enexexport1
This script parses through an Evernote ENEX file and converts the contents into individual files. Ok…it doesn't sound like much as Evernote has a similar feature built in, but none of the options really met my needs. So I developed my own solution and I’m posting it here in case anyone else wants to use it, tweak it, or whatever.

Why the script? Two reasons:

(1) I have a large number of notes (over 10,000) that are nothing more than document scans or PDF files. There's no other note content. Just the document that has been tagged accordingly for reference. 

As with any historical archive, organization is key. In EN I use this system;

Notes have at least two tags: Year/Month in format YYYY-MM and a category.

For example, the new dishwasher I purchased:

* the receipt would get scanned and tagged with: 
	* ```2020-10``` 		(the year/month purchased)
	* ```receipts``` 		(where all receipts get tagged)
	* ```home-inventory``` 	(need the receipt in case of warranty repair)
* the warranty documents get scanned and tagged:
	* ```2020-10```
	* ```home-inventory```
* the manual would either get scanned or (hopefully) downloaded from the manufactures website
	* ```2020-10```
	* ```home-inventory```
	* ```product-manuals```

This script saves the note attachments and appends the tags as part of the filename in the format:

```note_name [ tag1 tag2 tag3 ].pdf```

```scan00543 [ 2020-10 receipts home-inventory ].jpg```

(2) Convert the notes and use them in such a way that is independent of any proprietary notetaking or filing system. The notes and documents are converted from ENEX back into a basic filesystem, for which you can use any method for syncing; DropBox, OneDrive, NextCloud, Carbonite, your NAS storage, etc.

This method of tagging files is used by several note taking and organization applications:

TagSpaces - https://www.tagspaces.org/
sqauretag - https://github.com/mdom/squaretag

A similar concept but different format:
filetags - https://github.com/novoid/filetags


