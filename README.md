# alpine-consul-dns - Alpine Consul Container with BIND

## Available Tags

* ```0.6```,```latest``` (0.6/Dockerfile)

## Description
Extends the official Consul image to also include an installation of the BIND DNS server. BIND is setup to pass any ```*.consul``` DNS queries onto Consul but also perform public DNS resolution against Google's public DNS servers if needed. It's useful for performing development against a Consul server on a local machine. DNS queries can be directed to the container via the ```--dns``` Docker run argument.