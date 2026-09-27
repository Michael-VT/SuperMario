# 🍄 Super Mario — Edição DeepSeek

[English](README.md) | [Українська](README.UA.md) | [Русский](README.RU.md) | [Deutsch](README.DE.md) | [Français](README.FR.md) | **Português**

Um jogo de plataforma experimental no estilo Super Mario, reunido em **um único arquivo HTML**, criado junto com o chat de IA **DeepSeek**. Sem frameworks e sem build — basta abrir o arquivo no navegador e jogar.

> 🤖 **Sobre o experimento:** o jogo inteiro (HTML + CSS + JavaScript, ~1.770 linhas) foi gerado numa conversa com o DeepSeek e depois refinado. É publicado como exemplo de desenvolvimento de jogos com auxílio de IA. O log completo da conversa (`log.txt`) fica fora do repositório.

## ▶️ Como jogar

1. Baixe ou clone este repositório.
2. Abra `SuperMarioDeepSeek.html` em qualquer navegador moderno (Chrome, Firefox, Safari, Edge).
3. Digite o nome do jogador — e vamos lá!

Sem servidor, sem instalação, sem dependências.

## 🎮 Controles

| Ação | Teclado | Botão na tela |
|---|---|---|
| Iniciar / Pausar | `Espaço` | ▶ Iniciar / Pausar |
| Mover para a esquerda | `←` | ◀ Esquerda |
| Mover para a direita | `→` | Direita ▶ |
| Pular | `↑` | ⤒ Pular |
| Agachar (passar por baixo dos obstáculos) | `↓` | ⤓ Agachar |
| Reiniciar a corrida | `Esc` | ⟲ Reiniciar |

O movimento tem inércia: o Mario acelera enquanto você segura a direção e freia primeiro ao inverter o sentido — a sensação clássica.

## 🕹️ Jogabilidade

- O percurso com obstáculos, buracos e bônus é gerado no início de cada corrida.
- Colete os bônus: 🍒 cereja — **1 ponto**, 🍎 maçã — **2 pontos**, 🍯 mel — **3 pontos**.
- Perdeu um bônus? Você pode voltar e pegá-lo.
- Cair num buraco custa **1 de 3 vidas** ❤❤❤ — a corrida recomeça. Perder as três e o jogo começa de novo.
- Chegue à linha de chegada e ganhe um bônus de **10 pontos × vidas restantes**.

## 🏆 Tabela de pontuação e histórico

- A pontuação atual aparece acima do ranking.
- O **ranking top 10** fica ordenado, com a maior pontuação no topo (posição, nome, melhor pontuação).
- Quando sua pontuação entra no ranking, a entrada de menor pontuação sai.
- Os **últimos 10 jogos** aparecem numa lista separada.
- Tudo fica salvo no `localStorage` do navegador, então seu histórico continua lá na próxima vez.

> Observação: o idioma da interface do jogo é o russo.

## 🛠️ Tecnologia

- Um único arquivo autossuficiente: HTML + CSS + JavaScript.
- Renderização num `<canvas>` HTML5 (900 × 400).
- Persistência via `localStorage`.
- Os sprites dos bônus são desenhados por código — sem imagens.

## 🗺️ Roadmap

Este é o primeiro experimento. O plano é tentar criar **mais algumas variantes** do jogo com base nesta base de código.

## ⚖️ Licença

Distribuído sob a [Licença MIT](LICENSE) — uso, cópia, modificação e redistribuição gratuitos.

**Aviso:** este é um projeto de fã sem fins lucrativos, sem vínculo nem apoio da Nintendo. Todas as marcas relacionadas a Mario pertencem aos seus respectivos proprietários.
