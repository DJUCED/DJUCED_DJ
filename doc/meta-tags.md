# DJUCED Méta tags.

DJUCED uses meta tags to store informations into the media files
This document describes the meta tags used in DJUCED to store analysis results. 

# MP3 / WAV
DJUCED is using id3v2 tags by default but can read/write id3v1
## Id3v2 or id3v1 tags

|Field| ID |
|:--------|:-------|
| Title |TIT2|
| Artist|TPE1|
| Album |TALB|
| Genre |TCON|
| Comment |COMM|
| Year|TYER|
| Track |TRCK|

## Additional frames (only for id3v2)

|Field| Value |
|:----|:---|
|BPM|TBPM frame|
|Album  Artist|TPE2 frame|
|Composer|TCOM frame|
|Rating|POPM frame|
|Key|private GEOB frame DJUCED_KEY_DATA (int stored in an unsigned char vector)|
|CUE points|private GEOB frame DJUCED_CUE_DATA (encoded list a cue points encoded and stored in unsigned char vector)|
|First beat position|private GEOB frame DJUCED_FIRST_BEAT_DATA (double stored in an unsigned char vector)|
|Auto Gain|private GEOB frame DJUCED_GAIN_DATA (float stored in an unsigned char vector)|
|Energy|private GEOB frame DJUCED_DANCEABILITY (float stored in an unsigned char vector)|

# WMA
## Asf tags
| TAG |
|:----|
|Title
|Artist
|Album
|Genre
|Comment
|Year
|Track

## Addition attributes
|Field|Value|
|:----|:----|
|BPM|WM/BeatsPerMinute|
|Album Artist|WM/AlbumArtist|
|Composer|WM/Composer|
|Rating|POPM frame|
|Key|DJUCED/KEY (string encoded in base64 byte array)|
|CUE points|DJUCED/CUE-DATA (string encoded in base64 byte array)|
|First beat position|DJUCED/FIRST-BEAT (string encoded in base64 byte array)|
|Auto Gain|DJUCED/GAIN (string encoded in base64 byte array)|
|Energy|DJUCED/DANCEABILITY(string encoded in base64 byte array)|

# AIF, AIFF, AIFC
## Aif tags
| TAG |
|:----|
|Title|
|Artist|
|Album|
|Genre|
|Comment|
|Year|
|Track|

## Additional frames
|Field|Value|
|:----|:----|
|BPM|TBPM frame|
|Album  Artist|TPE2 frame|
|Composer|TCOM frame|
|Rating|POPM frame|
|Key|private GEOB frame DJUCED_KEY_DATA (int stored in an unsigned char vector)|
|CUE points|private GEOB frame DJUCED_CUE_DATA (encoded list a cue points encoded and stored in unsigned char vector)|
|First beat position|private GEOB frame DJUCED_FIRST_BEAT_DATA (double stored in an unsigned char vector)|
|Auto Gain|private GEOB frame DJUCED_GAIN_DATA (float stored in an unsigned char vector)|
|Energy|private GEOB frame DJUCED_DANCEABILITY (float stored in an unsigned char vector)|

# FLAC
## Vorbis Xiph Comment
| TAG |
|:----|
|Title|
|Artist|
|Album
|Genre
|Comment
|Year
|Track
## Addition fields:
|Field|Value|
|:----|:----|
|BPM|BPM |
|Album  Artist|ALBUMARTIST|
|Composer|COMPOSER|
|Rating|DJUCED_RATING_DATA|
|Key|DJUCED_KEY_DATA (base64 encoded in a byte array)|
|CUE points|DJUCED_CUE_DATA (base64 encoded in a byte array)|
|First beat position|DJUCED_FIRST_BEAT_DATA|
|Auto Gain|DJUCED_GAIN_DATA|
|Energy|DJUCED_DANCEABILITY (base64 encoded in a byte array)|
# Ogg Vobis
## Vorbis Xiph Comment
| TAG |
|:----|
|Title|
|Artist|
|Album|
|Genre|
|Comment|
|Year|
|Track|
## Addition fields:
|Field|Value|
|:----|:----|
|BPM|BPM |
|Album  Artist|ALBUMARTIST|
|Composer|COMPOSER|
|Rating|DJUCED_RATING_DATA|
|Key|DJUCED_KEY_DATA (base64 encoded in a byte array)|
|CUE points|DJUCED_CUE_DATA (base64 encoded in a byte array)|
|First beat position|DJUCED_FIRST_BEAT_DATA|
|Auto Gain|DJUCED_GAIN_DATA|
|Energy|DJUCED_DANCEABILITY (base64 encoded in a byte array)|

# M4A
## Fmp4 tags
| TAG |
|:----|
|Title|
|Artist|
|Album|
|Genre|
|Comment|
|Year|
|Track|
## Mp4 extra items
|Field|Value|
|:----|:----|
|BPM|----:com.GUILLEMOT.DJUCED:BPM (base64 encoded in a byte array)|
|BPM on iTunes|tmpo|
|Album  Artist||
|Composer|\251wrt|
|Rating|----:com.GUILLEMOT.DJUCED:RATING (base64 encoded in a byte array)|
|Key|----:com.GUILLEMOT.DJUCED:KEY (base64 encoded in a byte array)|
|CUE points|----:com.GUILLEMOT.DJUCED:CUE-DATA (base64 encoded in a byte array)|
|First beat position|----:com.GUILLEMOT.DJUCED:FIRST-BEAT (base64 encoded in a byte array)|
|Auto Gain|----:com.GUILLEMOT.DJUCED:GAIN (base64 encoded in a byte array)|
|Energy|----:com.GUILLEMOT.DJUCED:DANCEABILITY (base64 encoded in a byte array)|

# ANNEXE A
## DJUCED Keys
|KEY|Value|
|:--|:----|
|"A  Maj"| 0|
|"A# Maj"| 1|
|"B  Maj"| 2|
|"C  Maj"| 3|
|"C# Maj"| 4|
|"D  Maj"| 5|
|"D# Maj"| 6|
|"E  Maj"| 7|
|"F  Maj"| 8|
|"F# Maj"| 9|
|"G  Maj"| 10|
|"G# Maj"| 11|
|"a  min"| 12|
|"a# min"| 13|
|"b  min"| 14|
|"c  min"| 15|
|"c# min"| 16|
|"d  min"| 17|
|"d# min"| 18|
|"e  min"| 19|
|"f  min"| 20|
|"f# min"| 21|
|"g  min"| 22|
|"g# min"| 23|

