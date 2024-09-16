# DigitalOcean_Flask_Blog
Creating a Flask Blog with [DigitalOcean's Tutorial](https://www.digitalocean.com/community/tutorials/how-to-make-a-web-application-using-flask-in-python-3)

- - -

### Setting up a Project Environment
1. Create a designated project folder and change current working directory to it 
2. Create a virtual environment within the project folder and activate it:
```shell
python -m venv env
source env/bin/activate
```
### Testing a Small Base Application
1. In a empty file called `hello.py` add these lines of code and save it:
```python
from flask import Flask

app = Flask(__name__)

app.route('/')
def hello():
    return 'Hello World!'
```
2. Tell flask where to find the web application, `hello.py` and set it in development mode with:
```bash
export FLASK_APP=hello
export FLASK_ENV=development
```
3. Then run the application with:
```bash
flask run
```
4. Open the address in a web browser
