### 配置ssl
```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout tls.key -out tls.crt -subj "/CN=test.tv"
kubectl create secret tls test.tv --cert=tls.crt --key=tls.key
```
