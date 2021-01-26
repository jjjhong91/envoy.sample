# SSL證書
為example.com域名生成一個自簽的證書
```
$ mkdir certs; cd certs;
$ openssl req -nodes -new -x509 \
  -keyout example-com.key -out example-com.crt \
  -days 365 \
  -subj '/CN=example.com/O=youdianzhishi./C=CN';
  Generating a RSA private key
..+++++
.................................................................................................................+++++
writing new private key to 'example-com.key'
-----
$ cd -
```