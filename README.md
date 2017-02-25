# c7-systemd

A CentOS 7 System D base image

## Building

```bash
git clone https://github.com/aidanharris/c7-systemd c7-systemd
cd c7-systemd
sudo docker build --rm -t local/c7-systemd .
```

## Usage

```bash
> sudo docker run -d --rm --privileged --volume "/sys/fs/cgroup:/sys/fs/cgroup:ro" --volume /var/run/dbus/system_bus_socket:/var/run/dbus/system_bus_socket local/c7-systemd
944ba77d23c13f4938323c0cdde9a028e1117722e692cd52ce10fcde5985df37
> sudo docker exec -it 944ba77d23c13f4938323c0cdde9a028e1117722e692cd52ce10fcde5985df37 bash
```
