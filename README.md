# Docker Run With Watch

```
docker run -it \
  -p 3000:3000 \
  -v $(pwd):/app \
  -v /app/node_modules \
  -e CHOKIDAR_USEPOLLING=true \
  -e WATCHPACK_POLLING=true \
  cd8c791d7db5 \
  npm start
```