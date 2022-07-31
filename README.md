# seneye-unoffical-frontend

This is an alternative frontend to the seneye provided frontend. This is handy as you can actually refresh it just by reloading, something you can't easily do with the mobile app they provide.

This software is in a hideous unfinished state. Use at your own risk. It just about did the job for me, so I'm happy with it.

Run using nginx docker:

```
docker run --restart always --name seneye-nginx -p 8080:80 -v /ABSOLUTE/PATH/TO/seneye-unoffical-frontend/:/usr/share/nginx/html:ro -d nginx
```

The access : http://localhost:8080

In this fork:

Updated gauge js code to allow setting ranges of color in gauge
Added to just load the first device (I only have one, suits my needs)
Added auto full screen for device display (see: https://twitter.com/ProxiBlue/status/1553367729389809664)
