# appkit

Python 3 version of famous AppKit library to use in MacOs terminal


## Use:
```
#!/usr/local/opt/python@3.9/bin/python3.9
import logging
logging.basicConfig(filename='/tmp/act_window.log', level=logging.INFO, format='%(asctime)s - %(

try:
    from appkit import NSWorkspace
    activeAppName = NSWorkspace.sharedWorkspace().activeApplication()['NSApplicationName']
    print(activeAppName)
    logging.info(activeAppName)
except Exception as e:
    logging.error("{0}".format(e))
    print("Unknown")
```



 
