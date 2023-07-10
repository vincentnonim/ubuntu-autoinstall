# ubuntu-autoinstall

Clone this repository

Run container to host files
```
docker run -it --rm -p 80:80 -v $PWD/:/usr/share/nginx/html -d nginx
```

Insert following line in grub linux cmd line before ---
(some times need to escape the ; char)
```
autoinstall ds=nocloud-net\;s=http://container_ip/
```

