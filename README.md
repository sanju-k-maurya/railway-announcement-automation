# Railway announcement automation
CLI tool to automate announcement process of railway.

## Getting started
These instructions will give you an idea how project is working and generating announcement on your local machine. 

### Prerequisites
Python programming language

### Installing libraries

```
pip install pyaudio
pip install pydub
pip install gtts
pip install pandas
pip install xlrd==1.2.0
```
Note : xlrd version 1.2.0 has been used since updated version can't open .xlsx files.

Also install and configure ffmpeg.

### Initial files
```
main.py      (Python file to generate announcement)
railway.mp3  (mp3 file to get audio snippets )
announce_hindi.xlsx  (File containing list of trains whose announcement is generated)
```

### How to run
```
python main.py
```

Note : Make sure you are connected to internet since we are using gtts(Googel text to speech) library.
gtts is an easy tool to convert text to voice, but it requires an internet connection to operate because it depends entirely on Google to get the audion data.

After execution first intermediate .mp3 files will be generated.

Then individual announcement for each train present in the table(announce_hindi.xlsx) will be generated.
