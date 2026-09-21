## Método recomendado: Truncar los logs
1. Validar los tamanos de los logs de docker
```shell
$ sudo find /var/lib/docker/containers -type f -name '*-json.log' -exec du -h {} + | sort -hr
```

1. truncate -s 0 /var/lib/docker/containers/*/*.log
```shell
$ sudo find /var/lib/docker/containers/ -name "*.log" -exec truncate -s 0 {} \;
```
or
```shell
$ sudo find /var/lib/docker/containers/ -type f -name "*-json.log" -exec /usr/bin/truncate -s 0 {} \;
```
