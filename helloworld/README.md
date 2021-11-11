# Hello World

# Executar o programa
```
go run main.go
```

## Build e execução

```
go build main.go
```
Isso gera um executável no mesmo diretório, para executar:

```
./main
```

## Imports automáticos

Para importar automáticamente um pacote usado em seu código ao salvar o mesmo, é preciso ter instalado a ferramenta `goimports`

```
go get golang.org/x/tools/cmd/goimports
```