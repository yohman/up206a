# Setting up a local server

## Launch a terminal window
  - MacOS: go to spotlight, and type `terminal`
  - Windows 10: click the windows button, and type `command`
## Find out what version of Python you have installed
  ```python
  python -V
  ```
## Navigate to the directory you want to run your local server from
```python
cd Desktop
```
## 
```python
# If Python version returned above is 3.X
python3 -m http.server
# On windows try "python" instead of "python3", or "py -3"
# If Python version returned above is 2.X
python -m SimpleHTTPServer
```

Sample output:
```python
C:\Users\Yoh Kawano\Box Sync\htdocs>python3 -m http.server
Serving HTTP on :: port 8000 (http://[::]:8000/) ...
```
