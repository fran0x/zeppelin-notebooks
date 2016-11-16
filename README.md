# Zeppelin Notebooks

Web-based notebooks created with [Apache Zeppelin](https://zeppelin.apache.org/)

[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)

## Summary

This project contains notebooks created for:
- Research
- Exploratory Analysis
- Fast Prototyping

Additional information about the notebooks here available:
- Their main programming language is Scala / Spark (however other languages as Angular have been used as well)
- They can be visualized online by means of [ZeppelinHub](https://www.zeppelinhub.com) (see column *View* below)
- They require some libraries to be imported in the corresponding Interpreters (TODO: add new column for that)

## Notebooks

| Description	| Components | Code	| View |
| ------------- | ----- | ---------- 	| ------------  | --------  | --------  |
| Account Analysis | Spark | [json](https://github.com/flopezlasanta/zeppelin-notebooks/blob/master/2C17HCPG9/note.json) | [view](https://www.zeppelinhub.com/viewer/notebooks/bm90ZTovL2Zsb3Blemxhc2FudGEvWmVwcGVsaW4tTG9jYWwvOTkwMDU5MzNjYWZlNGVlMWJmZjk3MmYxYjNlMGVkMzEvbm90ZS5qc29u) |
| Twitter Streaming | Twitter / Spark Streaming / Angular / Leaflet | [json](https://github.com/flopezlasanta/zeppelin-notebooks/blob/master/2C3DZJWAT/note.json) | [view](https://www.zeppelinhub.com/viewer/notebooks/bm90ZTovL2Zsb3Blemxhc2FudGEvWmVwcGVsaW4tTG9jYWwvNzk5MzRjM2Q5NDFhNDhkYzlhMDQ2NWM2ZjlhNzIzY2Yvbm90ZS5qc29u) |

## Getting Started with Zeppelin

### Install Zeppelin (OS X)

1. Edit `/etc/hosts` adding your hostname: `127.0.0.1 localhost <hostname>`
2. Install Zeppelin: `brew install apache-zeppelin`
3. Start Zeppelin daemon: `./usr/local/Cellar/apache-zeppelin/0.6.2/bin/zeppelin-daemon.sh start`
4. Go to Zeppelin: `open http://localhost:8080`
5. Stop Zeppelin daemon: `./usr/local/Cellar/apache-zeppelin/0.6.2/bin/zeppelin-daemon.sh stop`

For simplicity add aliases to your bash profile, for instance the following:
- `alias zep="/usr/local/Cellar/apache-zeppelin/0.6.2/bin/zeppelin-daemon.sh start && open http://localhost:8080"`
- `alias zepx="/usr/local/Cellar/apache-zeppelin/0.6.2/bin/zeppelin-daemon.sh stop"`
- `alias zepl="tail -f /usr/local/Cellar/apache-zeppelin/0.6.2/libexec/logs/zeppelin-interpreter-spark-username-hostname.log"`

*Note: update 'username' and 'hostname' according to your system*

### Configure Zeppelin

- Enable GIT storage
- Enable user authentication (Shiro)
- Extend interpreters with additional libraries (Spark-Streaming-Twitter, jTDS...)

### Configure Zeppelin Hub

- Create account in Zeppelin Hub
- Download Zeppelin Hub library and include in Zeppelin installation
- Add new Zeppelin instance in Zeppelin Hub to obtain API token and user key
- Add API token and user key in Zeppelin shell script 
- Launch Zeppelin daemon

