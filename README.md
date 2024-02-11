Forked from -> https://github.com/trash/khinsider-mp3-downloader

# khinsider-batch-download

A script to crawl `http://downloads.khinsider.com/` for game soundtracks and download them. Downloads will be placed inside a `/downloads` directory inside the repo. Individual directories for each album will be generated automatically off the url name.

* Supports batch downloading of MP3, FLAC and any other file format

## Install
The only thing you need to install is python3: https://www.python.org/downloads/

## How To Use

### inputs.txt

#### Define inputs
Update the `inputs.txt` in the repo with a list of links, one link per line. 

The repo includes a properly formatted `inputs.txt` for reference.

#### Install Requirements
`pip install -r ./requirements.txt`

#### Run script
`python downloader.py`

#### Output
```python
PS C:\Users\stead\Documents\Coding Projects\khinsider-mp3-downloader> python downloader.py                      
[info] Input file found. Parsing for links...
[info] Url found: https://downloads.khinsider.com/game-soundtracks/album/fable-anniversary-gamerip        
[info] creating directory: downloads
[info] creating directory: downloads/fable-anniversary-gamerip
[info] crawling for links...
[info] 79 links acquired
[downloading] Music Bandit Camp.mp3 [7.38MB]
[done] "Music Bandit Camp.mp3"
[downloading] Music Bowerstone.mp3 [8.02MB]
[done] "Music Bowerstone.mp3"
[downloading] Music Chapel Of Evil.mp3 [4.44MB]
[done] "Music Chapel Of Evil.mp3"
```

### Input A URL Via CLI

If you'd prefer to manually enter URLs you can delete `inputs.txt` and then simply run `$ python3 downloader.py` from inside the repo and enter a link like 'http://downloads.khinsider.com/game-soundtracks/album/disgaea-3-raspberyl' (including the quotes) when prompted in the command line and hit enter.

