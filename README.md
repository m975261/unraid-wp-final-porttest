# unraid-wp-final-porttest

> Auto-containerized for Unraid 7.0.1 by **TITAN Dockerizer v2.8**
> Source: [https://github.com/howardchung/watchparty](https://github.com/howardchung/watchparty)

## Docker Image
```
docker pull muaeabudhabi/wp-final-porttest:latest
```

## Install on Unraid
1. Download `unraid-templates/my-wp-final-porttest.xml`
2. Copy to `/boot/config/plugins/dockerMan/templates-user/`
3. Docker tab → Add Container → select `wp-final-porttest`

## Auto-Updates
| Workflow | Schedule | Purpose |
|---------|----------|---------|
| `docker-build.yml` | Push / Manual / Dispatch | Builds multi-arch image → DockerHub |
| `upstream-watch.yml` | Daily 02:00 UTC | Checks upstream releases → triggers rebuild |
