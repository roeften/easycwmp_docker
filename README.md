# easycwmp_docker
Dockerfile for easycwmp (ubuntu)

You can override the following variables when building

For /etc/config/easycwmp:
-------------------------
URL: all instances url option will be replaced. Default http://127.0.0.1:7547/ (character | not allowed)
USERNAME: all empty instances of username will be replaced (character / not allowed)
PASSWORD: all empty instances of password will be replaced (character | not allowed)

For data model:
---------------
MODEL: either tr098 or  tr181 (default is tr098)

Example:
========
```
docker build --build-arg MODEL=tr181 --build-arg URL=http://myacs.example.com:/7547/ --build-arg USERNAME=user --build-arg PASSWORD=secret5 .
```

