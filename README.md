# 📱 Desafio POO - Modelagem e Diagramação de um Componente iPhone

Este projeto foi desenvolvido como parte do desafio proposto no bootcamp **Java Cloud Native** da DIO em parceria com o **Bradesco**, com o objetivo de aplicar os conceitos de Programação Orientada a Objetos (POO) e modelagem UML.

## 📋 Descrição do Desafio

Modelar um componente `iPhone` que possui três funcionalidades principais, com base na apresentação do iPhone em 2007:

- **Reprodutor Musical**
- **Aparelho Telefônico**
- **Navegador na Internet**

Cada funcionalidade foi representada como uma interface, sendo implementadas por uma única classe: `IPhone`.

---

## 🔍 Funcionalidades Modeladas

### 🎵 Reprodutor Musical
- `tocar()`
- `pausar()`
- `selecionarMusica(String musica)`

### 📞 Aparelho Telefônico
- `ligar(String numero)`
- `atender()`
- `iniciarCorreioVoz()`

### 🌐 Navegador na Internet
- `exibirPagina(String url)`
- `adicionarNovaAba()`
- `atualizarPagina()`

---

## 🧩 Diagrama UML

```mermaid
classDiagram

class ReprodutorMusical {
  +tocar()
  +pausar()
  +selecionarMusica(String musica)
}

class AparelhoTelefonico {
  +ligar(String numero)
  +atender()
  +iniciarCorreioVoz()
}

class NavegadorInternet {
  +exibirPagina(String url)
  +adicionarNovaAba()
  +atualizarPagina()
}

class IPhone {
  +tocar()
  +pausar()
  +selecionarMusica(String musica)
  +ligar(String numero)
  +atender()
  +iniciarCorreioVoz()
  +exibirPagina(String url)
  +adicionarNovaAba()
  +atualizarPagina()
}

ReprodutorMusical <|.. IPhone
AparelhoTelefonico <|.. IPhone
NavegadorInternet <|.. IPhone
