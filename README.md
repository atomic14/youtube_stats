# YouTube stats explorer

A silly little project for looking at successful (and unsuccessful) videos on a channel.

Stats may or may not be valid in any way...

# Setup

Project uses python, so make sure you've got python v3 installed.

Clone the repo and then run:

```
python -m venv venv
. ./venv/bin/activate
pip install -r requirements.txt
```

You can then either open the folder in vscode (assuming you have the python extension installed).

Or run

```
jupyter -notebook .
```

The interesting file is `youtube.ipynb` - change the channel URL to one you are interested in.

Change the channel name and channel URL:

```python
# we'll cached the channel vidoes in a json file with this name
CHANNEL_NAME = "great_scott"
# the channel URL
CHANNEL_URL = "https://www.youtube.com/channel/UC6mIxFTvXkWQVEHPsEdflzQ"
# how many videos to run against - more videos may give better stats
# but you'll be going further back in time so may be less relevant...
MAX_VIDEOS = 300
```