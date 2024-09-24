```sh
rm -rf ./build/* && npx -y @diplodoc/cli -i ./ -o ./build && npx -y http-server ./build --port=5099 --host=0.0.0.0
```