# slog
A simple logging package

## Install

```
pip install simlog
```

## Usage

```
import time
from simlog import SimLog


sLog = SimLog('./logs/log_file.txt')
sLog.log('这是第1条日志', end='\n')
sLog.log('这是第2条日志', console=False, end='\n')
sLog.info('这是第3条日志', end='\n')
sLog.info('这是第4条日志', console=False, end='\n')
time.sleep(3)
sLog.log(end='\n')
sLog.warning(end='\n')
sLog.info([[1,2,3], [2,3,4]], end='\n')
sLog.info({1:[1,2,3], 2:[2,3,4]}, end='\n')
sLog.error('error msg', end='\n')
sLog.critical('critical msg', end='\n')
time.sleep(3)
```