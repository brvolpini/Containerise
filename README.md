## Nginx Proxy

How to test the app:

clone the repo

    git clone https://github.com/brvolpini/Containerise.git
    cd Containerise

Run docker-compose in detach mode

```
docker-compose up -d
```

Testing if the proxy is working correctly

``` 
curl -k https://localhost
```

The result should be
``` 
It's easier to ask forgiveness than it is to get permission.
X-Forwarded-For: 172.20.0.1
X-Real-IP: 172.20.0.1
X-Forwarded-Proto: https
```
