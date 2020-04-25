# Vulnbox
Outdated Docker image based on Ubuntu 16.04, publicly exposing SSH and Nginx

# Build

```
sudo docker build . -t vulnbox
```

# Run

```
sudo docker run -d --rm -ti -p 2222:22 --name vulnbox vulnbox
```
