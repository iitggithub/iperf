A docker container running iperf. This is usually used to run the iperf client. If you want to run an iperf server, check out the iperf-server docker container.

# Supported Versions

iperf Version | Git branch | Tag name
--------------| ---------- |---------
2.0.9         | master     | latest
2.0.9         | 2.0.9      | 2.0.9

# Getting Started

Since this is only designed for once off use, here's how to use it.

```
docker run -it iitgdocker/iperf:latest -c iperf-server.example.com
```

# Environment Variables

Variable                 | Default Value (docker-compose) | Description
------------------------ | ------------------------------ |------------
TCP_WINDOW_SIZE          | unset                          | iperf can use this to set the TCP window size. You can also do this using ARGS as well

According to iperf --help, you can also set every single option using environment variables. ie IPERF_long option name, such as IPERF_BANDWIDTH.

# The End

If you have any comments, suggestions etc. Let me know.
