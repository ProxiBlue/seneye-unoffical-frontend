# seneye-unoffical-frontend

This is an alternative frontend to the seneye provided frontend. This is handy as you can actually refresh it just by reloading, something you can't easily do with the mobile app they provide.

This software is in a hideous unfinished state. Use at your own risk. It just about did the job for me, so I'm happy with it.

Run using nginx docker:

```
docker run --restart always --name seneye-nginx -p 8080:80 -v /ABSOLUTE/PATH/TO/seneye-unoffical-frontend/:/usr/share/nginx/html:ro -d nginx
```

The access : http://localhost:8080

In this fork:

* Updated gauge js code to allow setting ranges of color in gauge

example: 
PH < 7.0 is to low, so pink: 

![image](https://user-images.githubusercontent.com/4994260/182005344-d933a5f3-9ea0-4072-a31d-83358783b9f4.png)

PH > 7.0 < 8.0 = Green 

![image](https://user-images.githubusercontent.com/4994260/182005358-317529ca-5c30-4d0f-9408-950f96ad7a02.png)

PH > 8.0 is to high, red

![image](https://user-images.githubusercontent.com/4994260/182005384-d558b278-73b6-4bdc-b5bc-7fd342614f45.png)

Each gauge can now have own ranges with defined colors

* Added to just load the first device (I only have one, suits my needs)
* Added auto full screen for device display (see: https://twitter.com/ProxiBlue/status/1553367729389809664)
