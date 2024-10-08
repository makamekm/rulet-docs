```sh
rm -rf ./build/* && npx -y @diplodoc/cli -i ./ -o ./build/docs && npx -y http-server ./build --port=5099 --host=0.0.0.0 --cors
```

```sh
rm -rf ./build/* && npx -y @diplodoc/cli -i ./ -o ./_site/docs
DOCKER_BUILDKIT=1 docker build --platform linux/amd64 -t cr.yandex/crp66o1vj5ude8ip6mqa/rulet-2-ms-docs .
docker push cr.yandex/crp66o1vj5ude8ip6mqa/rulet-2-ms-docs:latest
```