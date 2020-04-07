# Configuration

This section you will learning the configure you application with Flask-vuejs extension.

## Introduction

Create the `.env` file in application root folder and set these environment variables.

```bash
FLASK_PATH_APPLICATION=app
FLASK_APP=app:create_app
FLASK_ENV=development
```

- **FLASK_PATH_APPLICATION**: You should set the application directory name. For example,
If you create the on `app` folder, you whould set this.
- **FLASK_APP**: Usually the people build your applications in the `app` folder and create the `__init__.py` file within the same directory.
Then, this variable should look like this: `FLASK_APP=app:create_app`. Read more about this in [here](https://flask.palletsprojects.com/en/1.1.x/cli/)
- **FLASK_ENV**: Set this according to your environment. [See](https://flask.palletsprojects.com/en/1.1.x/config/#environment-and-debug-features)

Install the python-dotenv library for manager this.

```bash
(.venv) $ pip install python-dotenv
```

Now, run the app:

```bash
(.venv) $ flask run
```

## Environment

You should know that for the vue cli working, your `FLASK_ENV` should be settled
as `development`. This occurred, because, on `production mode` the
vue-cli shouldn't work!

## Demo

You can see demo in [here](https://github.com/spadevs/integracao-vue-com-flask-live)
