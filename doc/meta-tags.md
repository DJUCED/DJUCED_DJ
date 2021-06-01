# DJUCED Méta tags.

DJUCED uses meta tags to store informations into the media files
# Standard tag
* ID3v2, ID3v1, WAV RIFF, WMA ASF, AIF/AIFF/AIFV RIFF, FLAC, OGG, M4A MP4

|Field| ID |
|:--------|:-------|
| Title |TIT2|
| Artist|TPE1|
| Album |TALB|
| Genre |TCON|
| Comment |COMM|
| Year|TYER|
| Track |TRCK|

# Extra tags
* ID3v2, APE, ID3v1
## Using FRAME

|Field| ID |
|:------------|:-------|
| BPM |TBPM| (BPM as string)
| Rating|POPM|
| AlbumArtist |TPE2|
| Composer|TCOM|


|Value | Frame | Name | Data|
|:-----|:------|:-----|:----|
| Key| GEOB| DJUCED_KEY_DATA| int stored as array of unsigned char|
| CUE points | GEOB| DJUCED_CUE_DATA| Cue data stored as array of unsigned char | (see Cue Data)
| First Beat | GEOB| DJUCED_FIRST_BEAT_DATA | double stored as array of unsigned char |
| Autogain | GEOB| DJUCED_GAIN_DATA | float stored as array of unsigned char|




