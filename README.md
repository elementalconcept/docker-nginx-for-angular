# docker-nginx-for-angular

Minimal nginx docker image with a configuration set to host
a single static front-end application behind a reverse-proxy
or to use on a local machine for development purposes.


## Usage

Inside your `Dockerfile` for nginx 1.15.12:

```
FROM elementalconcept/nginx-for-angular:1.15.12-alpine
```

Or to use nginx 1.16.0:

```
FROM elementalconcept/nginx-for-angular:1.16.0-alpine
```

Copy your files into `/usr/share/nginx/html`:

```
COPY /path/to/project/dist /usr/share/nginx/html/
```

Where `/path/to/project/dist` is the location of built assets in your local file system.
