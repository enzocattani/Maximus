# ⚔️ Erick Quest · 6º Ano

Jogo de estudo (Português + Inglês, 6º ano) feito para **celular**. O personagem **Erick** evolui conforme você acerta as questões. Funciona offline e pode ser instalado na tela inicial.

## Como funciona
- **4 abas embaixo:** 🧙 Herói · ⚔️ Missões · 🔥 Prova · 📖 Grimório.
- **9 eixos**, cada um ligado a um assunto. A cada 5 acertos o atributo sobe de nível:
  - 💪 Força: Substantivos
  - ⚡ Agilidade: Verbos
  - 🧠 Inteligência: Artigo, Adjetivo e Pronome
  - 🗣️ Carisma: Linguagem e Comunicação
  - 🎨 Criatividade: Textos e Gêneros
  - 🛡️ Coragem: Greetings & Pronouns
  - ✨ Magia: Verb To Be
  - 🍀 Sorte: Vocabulary (números, cores, família, dias, escola)
  - 🎯 Precisão: Articles & Demonstratives
- **Equipamentos:** Nível 3 em um atributo equipa algo no Erick (espada, escudo, capa, chapéu mágico...).
- **Combo:** 3 acertos seguidos = XP x2, 6 = XP x3.
- **🪄 50/50:** elimina duas alternativas erradas. Ganha-se subindo de nível, com sequência diária e abrindo baús.
- **🔥 Sequência diária:** voltar todo dia dá bônus de XP.
- **🎁 Baú:** missões com 80% ou mais de acertos liberam um baú-surpresa.
- **Grimório:** palavras-chave que se desbloqueiam ao acertar, com o resumo de cada assunto.
- **Treino de Erros:** refaz só o que errou.
- **Simulado Final:** 40 questões misturando todos os eixos, com nota, estrelas e pontos fracos.
- **Domínio por eixo:** mostra quanto de cada assunto já foi acertado.
- O progresso fica salvo no aparelho (localStorage).

## Publicar no GitHub Pages
1. Suba **todos** os arquivos deste repositório: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png` e `README.md`.
2. Em **Settings → Pages**, escolha *Deploy from a branch*, branch `main`, pasta `/ (root)`.
3. O jogo abre em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Instalar no celular
Abra o link no navegador do celular, toque no menu e escolha **“Adicionar à tela inicial”**. Vira um app em tela cheia.

## Adicionar questões
No `index.html`, adicione uma linha em `RAW`:

```js
["forca","Pergunta?","resposta certa","errada1|errada2|errada3","palavra-chave","explicação"],
```
Para verdadeiro/falso, use só uma errada: `"Verdadeiro","Falso"`.

Se atualizar o jogo e o celular mostrar a versão antiga, troque `V` em `sw.js` (ex.: `erick-quest-v3`).
