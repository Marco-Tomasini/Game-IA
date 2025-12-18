# Game-IA

> Coleção de jogos, experiências e experimentos feitos **apenas** com HTML, CSS e JavaScript (vanilla). Projetos pensados para aprender, compartilhar e empacotar ideias pequenas — tudo em arquivos simples, portáveis e fáceis de forkar.

[![License: MIT](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)

---

## Índice

* [Sobre](#sobre)
* [Demonstração](#demonstra%C3%A7%C3%A3o)
* [Recursos e características](#recursos-e-caracter%C3%ADsticas)
* [Como rodar localmente](#como-rodar-localmente)
* [Licença](#licen%C3%A7a)
* [Contato](#contato)

---

## Sobre

Este repositório reúne pequenos jogos, demos e experiments feitos **somente** com HTML, CSS e JavaScript (sem frameworks). A ideia é explorar o máximo possível do que dá para fazer com as tecnologias web "puras": motores simples, minigames, interfaces experimentais, puzzles, e protótipos visuais — todos pensados para serem fáceis de estudar, modificar e reaproveitar.
---

## Demonstração

🎮 **Jogue direto no navegador — sem download**

Este repositório possui uma página ativa no **GitHub Pages**, onde os projetos podem ser acessados diretamente:

🔗 **[https://marco-tomasini.github.io/Game-IA/](https://marco-tomasini.github.io/Game-IA/)**

* Cada jogo fica organizado em sua própria pasta.
* Basta clicar no projeto desejado para jogar.
* Compatível com navegadores modernos (Chrome, Edge, Firefox).

> Observação: alguns projetos experimentais ainda podem exigir teclado ou mouse específicos, descritos no README interno de cada jogo.

---

## Recursos e características

* Projetos em arquivos únicos (`.html`) ou pastas com recursos mínimos.
* Sem dependências externas (exceto assets como imagens e sons, quando necessário).
* Uso de:

  * DOM API e manipulação direta
  * Canvas 2D para gráficos e animações
  * Web Audio API para efeitos sonoros
  * CSS moderno (variáveis, grid/flex, animações)
* Pequenos motores reutilizáveis (input handling, game loop básico, colisões simples).
* Foco em performance e compatibilidade com navegadores modernos.

---

## Como rodar localmente

Opções rápidas:

1. **Abrir diretamente**

   * Alguns jogos são arquivos standalone. Dê duplo-clique em `index.html` para abrir no navegador.

2. **Servidor local (recomendado quando o projeto carrega assets via fetch)**

* Usando Python 3 (no diretório do projeto):

```bash
# Python 3
python -m http.server 8000
# então abra http://localhost:8000 no navegador
```

* Usando Node (http-server):

```bash
npm install -g http-server
http-server -p 8000
# abra http://localhost:8000
```

* Usando VS Code: instale a extensão **Live Server** e clique em "Go Live".

---

## Licença

Este projeto está disponível sob a licença **MIT**. Veja o arquivo `LICENSE` para detalhes.

---

## Contato

Se quiser feedback, revisão de código ou ajuda com um jogo específico, abra uma issue ou me chame via e-mail no seu perfil GitHub.