# Vulnbox
Outdated Docker image based on Ubuntu 16.04, publicly exposing SSH and Nginx

# Build

```
sudo docker build . -t vulnbox
```

# Run

```
sudo docker run -d --rm -ti -p 2222:22 -p 8000:80 --name vulnbox vulnbox
```

Nginx will be available at `http://127.0.0.1:8000`

```
curl http://127.0.0.1:8000
```

SSH will be listening at port `2222`, user is `root`, password is `THEPASSWORDYOUCREATED`
```
ssh -p 2222 root@127.0.0.1
```
