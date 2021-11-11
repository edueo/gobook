# Argumentos de linha de comando

A idéia desse programa é simular o comando `echo` do sistema operacionais baseado no Unix

```
go run echo.go Eduardo Alencar
```
Exibe `Eduardo Alencar` como saída


## os.Args

Armezena a lista de argumentos passados após o nome do programa


## Estrutura do for

```
for inicializacao; condição: pós {

}
```

No go não existe `while`, para simular o mesmo comportamento, podemos usar o `for`

```
for condicao {

}
```

loop infinito
```
for {

}
```

## Escrevendo o mesmo programa de outra forma

**Versão 2 **
```
package main

import (
	"fmt"
	"os"
)

func main() {
	s, sep := "", ""
	for _, arg := range os.Args[1:] {
		s += sep + arg
		sep = " "
	}
	fmt.Println(s)
}

```

**Versão 3**

```
func main() {
    fmt.Println(strings.Join(os.Args[1:], " "))
}
```
