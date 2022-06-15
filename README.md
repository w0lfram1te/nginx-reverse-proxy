# Reverse Nginx Proxy

Additional notes may be found on the related [post](https://w0lfram1te.com/deploying-nginx-reverse-proxy-on-docker).

## Quick Deployment 

1. Pull the repository.

```bash
git clone https://github.com/w0lfram1te/nginx-reverse-proxy
```

2.  Modify the relevant variables in the `docker-compose.yaml` file.  
	- `SERVER_NAME` - publicly exposed domain name that users will access
	- `PROXY_HOST`, `PROXY_PORT` - the host and port to forward traffic to

3. Deploy the entire thing under daemon mode using `docker-compose`.

```bash
docker-compose up -d
```