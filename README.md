# Template Python pronto para o HEROKU


## Dot Env
~~~.env
HOSTS = []
DEBUG = True
DATABASE_URL = sqlite://$(pwd)/db.sqlite3
~~~

## VSCODE
### Launch vscode
~~~.json
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Current File",
            "type": "python",
            "request": "launch",
            "program": "${file}/manage.py",
            "console": "integratedTerminal"
        },
        {
            "name": "Python: Django",
            "type": "python",
            "request": "launch",
            "program": "${workspaceFolder}/manage.py",
            "console": "integratedTerminal",
            "args": [
                "runserver",
                "--noreload"
            ],
            "django": true,
        },
        
    ]
}
~~~
