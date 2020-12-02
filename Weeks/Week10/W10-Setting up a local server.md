# Setting up a local server

## Launch a terminal window
  - MacOS: go to spotlight, and type `terminal`
  - Windows 10: click the windows button, and type `command`
## Find out what version of Python you have installed
  ```shell
  >python -V
  ```
If you do not have python, you will need to install it. If you are using Linux or macOS, it should be available on your system already. If you are a Windows user, you can get an installer from the [Python homepage](https://www.python.org/) and follow the instructions to install it.
  
## Navigate to the directory you want to run your local server from
```shell
>cd Desktop
```
## 
```shell
# If Python version returned above is 3.X
>python3 -m http.server
# On windows try "python" instead of "python3", or "py -3"
# If Python version returned above is 2.X
>python -m SimpleHTTPServer
```

Sample output:
```shell
C:\Users\Yoh Kawano\Box Sync\htdocs>python3 -m http.server
Serving HTTP on :: port 8000 (http://[::]:8000/) ...
```

## Run your local server
1. Open a browser window
1. type `http://localhost:8000/` (replace `8000` with the port number that was assigned in your previous step)

## Create an html document
1. Launch a text editor of your choice. The two I recommend are [Sublime Text](https://www.sublimetext.com/) and [Atom](https://atom.io/).
1. Create some html content:
```html
<h1>Hello World</h1>
<p>
  My three favorite things:
  <ol>
    <li>sushi</li>
    <li>ramen</li>
    <li>maps</li>
  </ol>
</p>
```
1. Save the file and name it `hello.html` (no spaces). Make sure to save it in the same directory you launched your local server in.
1. Open a broswer window, and enter `http://localhost:8000/hello.html`
