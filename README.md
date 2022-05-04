# flaskr

# Run
To run this program you have to open the directory which it is located in, my case:
```
$ cd projects
$ cd flask-tutorial01
$ cd TEST
```
You then must create a virtual environment:
```
$ python3 -m venv venv
```
Then use the following commands to activate the virtual environment and run the program:
```
$ . venv/bin/activate
$ export FLASK_APP=flaskr
$ export FLASK_ENV=development
$ flask init-db
$ flask run
```

Alternatively you can run the setup_flaskr.env file after creating the virtual environment:
```
$ ./setup_flaskr.env
```

After that, open http://127.0.0.1:5000/auth/login.
If and error returns saying ```OSError``` this means that another program is already using port 5000
You can either identify and stop the other program, or use the following command to pick a different port:
```
$ flask run --port 5001
```

This should lead you to a page asking for a login!

