# Demonstration

![Demo](https://raw.githubusercontent.com/jafarlihi/file-hosting/master/rssnix-demo.gif?raw=true)

# Installation

`git clone https://github.com/jafarlihi/rssnix --depth=1 && cd rssnix && go install`

# Command line flags

`config`
- Opens config file with $EDITOR

`update [feed]`
- If [feed] argument is given and is space-delimited list of feeds, then these feeds are updated
- If no [feed] argument is given then all feeds are updated

`open [feed]`
- If [feed] argument is given then the said feed's directory is opened with the configured viewer
- If no [feed] argument is given then the general feeds directory is opened with the configured viewer

`add [feed name] [feed url]`
- Adds a new feed to the config file

# Sample config file

```
[settings]
default_viewer = vim
feed_directory = ~/rssnix

[feeds]
CNN-Tech = http://rss.cnn.com/rss/edition_technology.rss
HackerNews = https://news.ycombinator.com/rss

(Tip: ranger is another great canditate for default_viewer)
```
