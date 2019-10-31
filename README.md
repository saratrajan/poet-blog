## Installation

Read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.

### Test your site locally

In order to see your site in action, run Hugo's built-in local server. 

Build it first:

```bash
$ hugo
```

.. and then start the server:

```bash
$ hugo server -w
```

Now launch `http://localhost:1313` on your browser.


## Fan of Docker Containers?
You can quickly containerize this using `nginx` as below (after building):
```docker
FROM nginx:1.17.5-alpine
COPY public/ /usr/share/nginx/html/
```


## Credits
This is using `One-Day-Only (OneDly) Project Theme` as template. Check out the cool theme [here](https://github.com/cdeck3r/OneDly-Theme).