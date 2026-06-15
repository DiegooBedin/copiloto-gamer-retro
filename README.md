# 🎮 DB Games: Copiloto de Vendas com IA para Consoles e Colecionáveis

Este repositório contém o projeto do **Copiloto de Vendas com IA da DB Games**, desenvolvido como entrega para o Desafio Criativo da plataforma **DIO (Digital Innovation One)**.

A **DB Games** é uma loja fictícia especializada na venda de consoles de videogame dedicados (de mesa e portáteis), jogos físicos originais de época, periféricos e **artigos colecionáveis oficiais** (como action figures licenciadas, luminárias LED temáticas e quadros de decoração gamer).

---

## 🎯 Definição do Projeto

* **Tema Escolhido:** Loja Gamer de Consoles (Mesa, Portáteis) e Artigos Colecionáveis.
* **Usuário Principal:** Vendedores e atendentes comerciais da DB Games (WhatsApp, Instagram Direct ou balcão).
* **Problema que Resolve:** Agiliza o atendimento, auxilia no contorno de objeções difíceis (como originalidade de Action Figures, utilidade de consoles físicos vs. emuladores, compatibilidade em TVs modernas e garantia de usados) e ajuda a realizar vendas casadas (cross-selling) de colecionáveis e acessórios para elevar o faturamento da loja.
* **Abordagem Adotada:** **Copiloto de IA** (um assistente de retaguarda que apoia o vendedor humano em vez de conversar diretamente com o cliente final).

---

## 📠 Catálogo de Consoles Suportados (Base de Dados)

O repertório do Copiloto é completo e abrange os seguintes consoles:

* **Sony PlayStation:** PlayStation 5 (Slim), PlayStation 4 (Slim/Pro), PlayStation 3, PlayStation 2, PlayStation 1, PSP e PS Vita.
* **Nintendo:** Nintendo Switch (OLED/Lite), Wii U, Wii, GameCube, Nintendo 64, Super Nintendo (SNES), NES (Nintendinho), Nintendo 3DS/2DS, Nintendo DS, Game Boy Advance SP, e Game Boy Color/Classic.
* **Sega:** Dreamcast, Sega Saturn, Mega Drive, Master System e Sega Game Gear.
* **Atari:** Atari 2600.

---

## 🗂️ Estrutura do Repositório

* `prompts/copiloto.txt`: Contém o **Prompt de Sistema** que define a persona, o tom de voz e as regras de negócio que a IA deve seguir.
* `knowledge/produtos.md`: Catálogo detalhado e completo dos consoles, portáteis, colecionáveis, jogos e periféricos vendidos, com preços e argumentos de vendas.
* `knowledge/objecoes.md`: Guia de argumentos prontos para contornar hesitações comuns dos clientes.
* `knowledge/faq.md`: Respostas rápidas sobre formas de pagamento, garantia, frete e trocas.

---

## ⚡ Exemplo Prático de Uso (Simulação)

### Cenário 1: Dúvida sobre Console Retrô & Emulação
* **📥 Entrada do Vendedor:** 
  > *"O cliente perguntou se o Game Boy Advance SP de R$ 600,00 vale a pena, já que ele pode jogar em um emulador de celular de graça. O que eu respondo?"*
* **🤖 Resposta do Copiloto:**
  * **🧠 ANÁLISE DA SITUAÇÃO:** O cliente compara o console físico ao emulador de celular. Devemos focar na experiência tátil original (botões físicos, formato dobrável do GBA SP), na tela retroiluminada de fábrica e na nostalgia/colecionismo de ter o aparelho físico em mãos, citando a garantia de 3 meses da loja.
  * **💬 RESPOSTA SUGERIDA (Copie e Cole):** 
    > "Fala, gamer! Tudo bem? Cara, jogar no emulador de celular é legal para quebrar um galho, mas nada se compara à experiência de ter o Game Boy Advance SP de verdade nas mãos! O toque dos botões físicos originais, o design dobrável icônico e a tela iluminada dão uma sensação única que o toque na tela lisa do celular não consegue reproduzir. É ter um pedaço da história dos videogames com você! 🎮 e o melhor: nosso GBA SP é totalmente restaurado, higienizado, com bateria testada e vai com 3 meses de garantia de loja para você jogar sem preocupação. Vamos garantir essa máquina nostálgica?"
  * **🚀 PRÓXIMA AÇÃO:** Sugerir ao vendedor perguntar qual jogo clássico marcou a infância do cliente (ex: Pokémon, Mario ou Zelda) para engajá-lo e oferecer o frete grátis se for para o Sul/Sudeste (já que o valor de R$ 600,00 ultrapassa o frete grátis de R$ 500,00).

### Cenário 2: Pegadinha de Placa de Vídeo / Computador (Restrição de Escopo)
* **📥 Entrada do Vendedor:** 
  > *"Um cliente mandou no WhatsApp: 'opa, vcs trabalham com placa de vídeo? tô precisando de uma RTX 4060 ou ver se vcs montam um pc gamer completo pra mim rodar o gta 5'."*
* **🤖 Resposta do Copiloto:**
  * **🧠 ANÁLISE DA SITUAÇÃO:** O cliente está solicitando peças de PC/Informática. Nossa regra de negócio proíbe estritamente a venda de hardware de PC. Devemos declinar educadamente informando nosso foco em consoles dedicados, e redirecioná-lo para os consoles modernos de alto desempenho (PS5 / Xbox Series X) que rodam GTA V de forma perfeita e barata.
  * **💬 RESPOSTA SUGERIDA (Copie e Cole):** 
    > "Opa, tudo bem? Rapaz, nós não trabalhamos com peças de computador, placas de vídeo ou montagem de PCs. Nosso foco total aqui na DB Games são consoles de videogame dedicados e colecionáveis oficiais! Se você quer rodar o GTA V e os últimos lançamentos com gráficos incríveis sem a dor de cabeça de montar e configurar um PC, nós temos o PlayStation 5 e o Xbox Series X novos em estoque com 1 ano de garantia! Eles rodam os jogos mais pesados com um custo-benefício incrível. Quer que eu te mande os valores deles?"
  * **🚀 PRÓXIMA AÇÃO:** Oferecer os valores do PS5 Slim (a partir de R$ 3.800,00 no Pix com 5% de desconto) ou Xbox Series X.

---

## 🧪 Roteiro de Testes (10 Mensagens para Validar a IA)

Você pode testar a inteligência do copiloto copiando as seguintes mensagens fictícias no ChatGPT ou Gemini após carregar as regras e a base de conhecimento:

1. **Sobre Portátil Retrô:** *"oii, vi q vcs tem o game boy advance sp. a tela dele ta com mto risco? a carcaça é original ou vcs trocaram? manda foto pfvr"*
2. **Sobre Action Figures (Tamanho/Escala):** *"Gostei muito desse Zoro da Banpresto que tá no site, mas não entendo nada de escala kkkk ele tem quantos centímetros de altura mais ou menos? Fica bem na estante?"*
3. **Sobre Consoles de Geração Atual:** *"Boa tarde. O PS5 de vcs é o modelo Slim? Vem com quantos controles? E como funciona a garantia com vcs se der algum problema?"*
4. **Sobre Autenticidade de Estátuas:** *"Olá, esse Funko Pop do Darth Vader é original msm? Pergunto pq quebrei a cara na internet umas semanas atrás com pirata. A caixa dele tá lacrada e sem amassado? Sou bem chato com isso rs"*
5. **Sobre Especificações Técnicas de Luminárias:** *"Eaí blz? Essa luminária do logo do playstation funciona na tomada ou é só pilha? Se for cabo, vcs mandam junto a fonte ou é só o fio?"*
6. **Sobre Sugestão de Presente (Cross-sell):** *"Oi pessoal, preciso de uma ajuda. Quero dar um presente de aniversário pro meu namorado, ele joga muito o Nintendo Switch e ama Zelda. Vcs tem alguma opção de decoração ou quadro dele até uns 150 reais?"*
7. **Sobre Jogos de Gerações Passadas:** *"Gente, o jogo do PS2 que vcs tão vendendo (o GTA San Andreas) é mídia física original né? Roda de boa se o meu PS2 for bloqueado?"*
8. **Sobre Materiais de Decoração:** *"Gostei do quadro do mapa de Elden Ring. Ele já vem com aquela moldura de madeira preta ou é só a placa? E pra pendurar, precisa furar a parede?"*
9. **Pegadinha de Hardware/Informática:** *"opa, vcs trabalham com placa de vídeo? tô precisando de uma RTX 4060 ou ver se vcs montam um pc gamer completo pra mim rodar o gta 5"*
10. **Sobre Compra Combinada e Frete:** *"Queria fechar o Nintendo Switch Lite com vcs e aproveitar pra pegar tbm o action figure do Mario pra economizar no frete, vcs conseguem mandar tudo no mesmo pacote?"*
