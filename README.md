> cordova-web-platform-tests

# why

to test W3C API specification adherence by cordova platforms

# wat

A cordova shell app to be used in conjunction with the
[W3C's web-platform-tests](https://github.com/w3c/web-platform-tests).

# how

1. configure and run the server that comes w/ web-platform-tests
  - set up your `/etc/hosts` file as per web-platform-tests README. Make sure
    you can run the server via `./wpt serve`.
  - copy `config.default.json` to `config.json`, and set the `host` property to
    an internal network IP accessible by a phone or emulator/simulator.
  - ensure this IP is used in the `/etc/hosts` file as per above
2. replace all the IP references in config.xml
3. build + run the app via `cordova run`

