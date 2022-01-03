# Chromium Headless Trunk

Using the binary from the Chromium snapshot bucket

```
$ docker run -d --rm -p=127.0.0.1:9222:9222 \
 --memory="250m" --cpu-shares="700" \
 --name=chrome-headless \
 -v /tmp/chromedata/:/data mpdroog/chrome
```

Inspired by
- [alpeware](https://github.com/alpeware/chrome-headless-trunk)
- [beaufortfrancois](https://github.com/beaufortfrancois/download-chromium)
- [National Library of Norway](https://github.com/nlnwa/docker-chrome-headless)

This fork adds hide-scrollbars to the chrome-daemon shellscript and
 limits memory+CPU by default.

