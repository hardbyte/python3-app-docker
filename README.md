Inspired by [google/python-runtime][1] this docker image makes it easy to deploy a standard Python 3 application.

Unlike Google's Docker image this inherits from Ubuntu.

Similar notes to python-runtime, just make a `Dockerfile`:


    FROM hardbyte/python3-app


 - Expects a `requirements.txt` file
 - assumes your app listens on port 8080
 - either has a `main.py` or defines `ENTRYPOINT ["/env/bin/python/", "/app/other.py"]

  [1]: https://registry.hub.docker.com/u/google/python-runtime/%20google/python-runtime

