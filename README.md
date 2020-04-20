# gistat easy way to get statistics from https://gismoldova.maps.arcgis.com

## Usage
Here I will describe how to use it.

###  Getting it
To download gistat, either fork this github repo or simply use Pypi via pip.
```sh
$ pip install gistat
```
### Requirements
gistat using selenium and geckodriver.
You need to download latest version of it from https://github.com/mozilla/geckodriver/releases and extract into root of your project.

### Using it
```Python
import gistat

with gistat.GiStat() as stat:
    print(stat.get_general_stat())
```
Other usage you will find in examples.py