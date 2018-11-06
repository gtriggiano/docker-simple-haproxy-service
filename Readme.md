# Simple HAProxy Service

```bash
# pull image
docker pull gtriggiano/simple-haproxy-service

# run the proxy
docker run -d \
  -p "8080:8080" \
  -e "BIND_PORT=8080" \
  -e "TARGET_HOST=google.com" \
  -e "TARGET_PORT=80" \
  gtriggiano/simple-haproxy-service
```
