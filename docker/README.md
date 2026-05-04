## Método recomendado: Truncar los logs
1. truncate -s 0 /var/lib/docker/containers/*/*.log
```shell
$ sudo find /var/lib/docker/containers/ -name "*.log" -exec truncate -s 0 {} \;
```
