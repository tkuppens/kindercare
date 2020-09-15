kindercare_sync
===============

Download pictures and videos with metadata for archiving from the Kindercare website (Himama platform)

Description
-----------

Sync utility for kindercre media. Local id db (file: id.db) makes sure that you only download the media files you did not download already. 

child id

You need to provide your child's id in the script. See Manage Children page: https://classroom.kindercare.com/accounts . The ID is in the url : https://classroom.kindercare.com/accounts/xxxxxx 


cookie

Cookiefile has to be called cookies.txt and has to be in the same dir as the kcsync script.
Must contain the Netscape-style cookie.  _himama_session (has a long expiration date, so you only need to provide it ones. By the time it expires your little one will be in college)


Use
---

kcsync -ci 

	-i : ignore db - id of downloaded media is not added to the local db
	-c : metadata activity information is added as  caption below the picture.


Dependencies
------------

	- jq
	- exiftool
	- ImageMagick (convert)
	- ffmpeg
	- wget
 
