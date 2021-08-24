### Create user test/test
```
htpasswd -c auth.db anthony
```
### Create user test2/test2
```
htpasswd auth.db test2
```
### Get encrypted string
```
base64 auth.db
```
### IngressRoute add middlewares filed
```
apiVersion: traefik.containo.us/v1alpha1
kind: IngressRoute
metadata:
  name: ingressroute
spec:
# more fields...
  routes:
    # more fields...
    middlewares:
      - name: test-auth
```
