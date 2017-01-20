# zappa-django-lambda
Project template for Django Rest Framework running on AWS Lambda with Zappa

# Local development
```
$ sudo pip install virtualenv
$ virtualenv --no-site-packages bcfs
$ source ./bcfs/bin/activate
(bcfs)$ cd server/
(bcfs)$ pip install -r requirements.txt
(bcfs)$ ./manage.py runserver 0.0.0.0:8000
```

# Deploy
- Make sure you have a `~/.aws/credentials`
```
(bcfs)$ zappa deploy dev|stage|prod
```

# Get logs
```
(bcfs)$ zappa tail
```

Visit https://github.com/Miserlou/Zappa to learn more about Zappa
