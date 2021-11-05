简介: 用 golang 写的 http server,支持 VUE SPA, history 模式,刷新不会404

# go mod init go_preview
# go get -v -u github.com/gorilla/mux


# 打包 windows exe
GOOS=windows GOARCH=386 go build -o main.exe main.go

# 64-bit
GOOS=linux GOARCH=amd64 go build -o bin/app-amd64-linux main.go

# 32-bit
GOOS=linux GOARCH=386 go build -o bin/app-386-linux main.go

# 运行目录结构如下:
```
├── dist
│   └── index.html
├── main.exe
```

双击  main.exe 即可运行