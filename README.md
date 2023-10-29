# gowasm

## build

```sh
    GOOS=js GOARCH=wasm go build -o assets/main.wasm cmd/wasm/main.go
```

## run

```sh
    go run cmd/server/main.go
```

## todo
- build a very lightweight tool that essentially runs like npm or yarn
- it should enable you to do a one liner like `gowasm dev` and make a watcher for your site.
- it should be a standalone tool. that has it's own repo.
- it should be installed with go install (maybe go get)
- it should also support `gowasm build` and that should generate a dist/ folder with a classic minified html,css,js but also main.wasm  (can't get much smaller than binary)
- it should get rid of the need for the developer to have the assets folder (that is the developer should just be writting go code)
