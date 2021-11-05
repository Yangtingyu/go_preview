用 golang 写的 http server,支持 vue spa history 模式,刷新不会404

go mod init go_preview
go get -v -u github.com/gorilla/mux


<!-- 打包 windows exe -->
GOOS=windows GOARCH=386 go build -o main.exe main.go