# Desafio-UML
# [DIO](www.dio.me) - Trilha Java Básico

## Autores
- [Luiz_Oliveira](https://github.com/LuizzOliveira)

## POO - Desafio

### Modelagem e Diagramação de um Componente iPhone

Modelar e diagramar a representação UML do componente iPhone, abrangendo suas funcionalidades como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.


#### Funcionalidades a Modelar
1. **Reprodutor Musical**
   - Métodos: `tocar()`, `pausar()`, `selecionarMusica(String musica)`
2. **Aparelho Telefônico**
   - Métodos: `ligar(String numero)`, `atender()`, `iniciarCorreioVoz()`
3. **Navegador na Internet**
   - Métodos: `exibirPagina(String url)`, `adicionarNovaAba()`, `atualizarPagina()`

### Objetivo
 Criar um diagrama UML que represente as funcionalidades descritas acima.

###Diagrama UML (Mermaid)
```mermaid
classDiagram
    class ReprodutorMusical {
	<<interface>>
        +ligar() : void
        +pausar() : void
        +selecionarMusica(String musica) : void
 }
    class AparelhoTelefonico {
	<<interface>>
        +exibirPagina(String url) : void
        +adicionarNovaAba() : void
        +atualizarPagina() : void   
    }
    class  NavegadorInternet {
	<<interface>>
        +ligar(String numero) : void
        +atender() : void
        +iniciarCorreioVoz() : void    }
    class iPhone {
    }
    ReprodutorMusical <|-- iPhone
    AparelhoTelefonico <|--iPhone
    NavegadorInternet <|--iPhone
```

```bash
https://github.com/LuizzOliveira/trilha-java-basico/desafios/poo/README.md
```` 
