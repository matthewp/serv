Serv
====

Ad hoc serving of HTTP requests from any directory.

    $ npm install -g serv
    $ cd directory/to/serv
    $ serv
    Serving files from directory/to/serv at http://localhost:8000
    Press Ctrl+L to launch in browser
    Press Ctrl+C to quit

By default, serv only allows access from the local machine. This protects your
file system from external network access. If remote access is needed, you may
specify an IP address to bind to with the `-b` flag, or `--public` to allow all
network access. Access may still be limited by your machine's firewall.

    $ serv -h
    Options:
      -h, --help  Show this help message                               [boolean]
      -b, --bind  IP to bind the server to                             [default: "127.0.0.1"]
      -p, --port  Port to bind the server to, uses PORT env var if set [default: "Auto (8000+)"]
      --path      File system path to expose                           [default: <current working directory>]
      --public    Listen on all available IP addresses                 [boolean]
