# Saludos en GO | Greetings on GO

Este paquete proporciona varios saludos en GO, es de mis primeros intentos, así que agradecería mucho cualquier consejo.
This package provides several greetings in GO, it is one of my first attempts, so any advice would be greatly appreciated.

## Instalación | Installation: 

Ejecuta el siguiente comando para instalar el paquete | Run the following command to install the package: 
```bash
go get -u github.com/drunw/greetings
```

## Como usarlo? | How to use it?

Aqui tienes una forma para usar el paquete | Here is a way to use the package: 

```go 
package main

import (
	"fmt"
	"log"

	"github.com/drunw/greetings"
)

func main() {
	message, error := greetings.Hello("")
	if error != nil {
		log.Fatal(error)
	}
	fmt.Println(message)
}
```
