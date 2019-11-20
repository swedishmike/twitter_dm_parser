# Twitter DM Parser

### Background
For, _ahem_, a specific reason I found myself wanting/needing to be able to import DM data from a Twitter backup.

The file format was a bit weird, it looked a bit like Json but it wouldn't import straight in like that.

First I tried to ask for help on [Twitter](https://twitter.com/swedishmike/status/1196750124636147712) but that didn't really work out so I went Googling...

I found the following [blog] (http://www.farleyforensics.com/2018/10/01/twitter-archive-parser-analysis/) which lead me the the accompanying [GitHub Repo](https://github.com/jfarley248/Twitter-Archive-Parser).

The code was for Python 2 and I also wanted to get this into a Pandas dataframe for further analysis and data wrangling so I happily stole the code and changed it to suit my needs. Another decision I made was to move it into a Jupyter Notebook in order to be able to play with data on the fly a bit easier.

Big thanks to [Jack Farley](https://twitter.com/jackfarley248) for the original idea and code!

### What does it do?
Not much really. But what it does do it seems to do fairly well.

It will parse the **direct-message.js** and **direct-message-group.js** files from a Twitter backup. The end product(s) you'll end up with are the combined data in a Pandas dataframe as well as in a exported csv file.

The location of the archive files as well as the name and location of the exported csv file are defined as variables in the Notebook so you can customise that fairly easily.

### Feedback

If you have any feedback/bugs/improvements etc - open an Issue here on Github or submit a pull request. As we all know: _Sharing is caring!_


### TO-DO
- Automagically iterate through all ID's and pull in the corresponding Twitter user names and populate the dataframe/csv file with those.
