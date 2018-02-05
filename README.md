# Mary
Mary is a python application which provides a sumMARY of your IRC session. Mary was written in Python 3.6.3 and includes a simple, lightweight, self-contained implementation of the IRC protocol suitable for the use cases of this application.

# Dependencies
Wordclouds are generated using the [WordCloud](https://github.com/amueller/word_cloud) Python module. Mary uses the following Python Standard Library modules:

`time
signal
string
os
operator
socket
asyncio
re `

Mary was tested on the Python 3.6.3 interpreter so this version is recommended for execution.

# User Stories
1. As a [Twitch](http://www.twitch.tv) streamer, I want to get a summary of my chat history of my viewers so that I can understand the discussion without having to read the entire chat history.
2. As an IRC user, I want to create a wordcloud of based on chat messages in a chatroom so that I can use it as art.
3. As a moderator of an IRC channel, I want to get word frequencies on my IRC chat channel so that I can moderate my channel without having to read the entire chat history.
4. As an IRC user, I want to understand the [sentiment](https://en.wikipedia.org/wiki/Latent_semantic_analysis) of an IRC channel.

# Limitations
Mary does not handle nickname registration. If your channel requires nickname registration, you must register before using Mary on that channel.

# Versions
Version 1 (the current version) supports User Stories 1 and 2 only. User Stories 3 and 4 are planned for a future version

# Usage
Mary can be executed on the command line using the python interpreter. Once running, Mary will collect chat messages. Upon receipt of a SIGHUP, Mary will output two things:
* An order list of terms and their frequencies
* A wordcloud in .png format (wc.png in the directory that the script is running in)

# Example
`$ python mary.py
$ killall -HUP python`

# Code
Code will be furnished upon request
