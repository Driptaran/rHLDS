# rHLDS
This library allows you to use Half-Life RCON protocol.

## REQUIREMENTS
Python 3+

## INSTALLATION
```
pip3 install rHLDS
```
Or from git:
```
pip3 install git+https://github.com/chmod1/rHLDS.git
```

## USING
```python
from rHLDS import Console

# Default port 27015
srv = Console(host='127.0.0.1', password='somePass')
# If you need another port
srv = Console(host='127.0.0.1', port=27016, password='somePass')

# Connect to server
srv.connect()

# Execute any command
print(srv.execute("status"))

# Сlose connection
srv.disconnect()
```

# LICENSE
[MIT License](http://www.opensource.org/licenses/MIT)
