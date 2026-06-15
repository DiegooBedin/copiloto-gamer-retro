# 🎮 DB Games — Copiloto de Vendas com IA para Atendimento ao Cliente

Projeto desenvolvido como parte do desafio **“Copiloto de Vendas com IA para Atendimento ao Cliente”**, da **DIO (Digital Innovation One)**.

A proposta deste projeto é demonstrar como a Inteligência Artificial pode apoiar uma pessoa vendedora durante o atendimento, ajudando a entender melhor o cliente, organizar informações, responder dúvidas, lidar com objeções e sugerir próximos passos comerciais.

---

## 📌 Tema Escolhido

O tema escolhido foi uma **loja gamer fictícia**, chamada **DB Games**.

A DB Games é especializada em:

* consoles de videogame atuais;
* consoles retrô;
* consoles portáteis;
* jogos físicos;
* controles e acessórios;
* action figures licenciadas;
* luminárias LED temáticas;
* quadros e itens decorativos gamer.

A loja tem foco em produtos ligados a **consoles, nostalgia, colecionismo e cultura gamer**.

---

## 👤 Usuário Principal da Solução

O usuário principal da solução é o **vendedor ou atendente comercial da DB Games**.

Esse vendedor pode atuar em canais como:

* WhatsApp;
* Instagram Direct;
* atendimento online;
* atendimento presencial no balcão da loja.

A IA não foi criada para substituir o vendedor. Ela funciona como um **copiloto de atendimento**, ou seja, uma ferramenta de apoio para ajudar o vendedor a responder melhor e conduzir a conversa com mais segurança.

---

## ❗ Problema de Vendas e Atendimento

Durante um atendimento comercial, o vendedor pode receber dúvidas muito diferentes, como:

* cliente comparando console físico com emulador;
* dúvida sobre garantia de console usado;
* medo de comprar action figure falsa;
* pergunta sobre compatibilidade de consoles antigos com TVs modernas;
* pedido de produtos que a loja não vende, como placa de vídeo ou montagem de PC gamer;
* cliente interessado em um produto fora de estoque;
* necessidade de sugerir acessórios ou produtos complementares.

O problema é que, sem uma orientação clara, o atendimento pode ficar inconsistente, demorado ou pouco estratégico.

Este projeto resolve esse problema ao criar um copiloto que ajuda o vendedor a:

* interpretar a dúvida do cliente;
* identificar a melhor abordagem comercial;
* sugerir uma resposta pronta para envio;
* indicar uma próxima ação para continuar a venda;
* manter o atendimento dentro das regras da loja.

---

## 🧠 Abordagem Utilizada

A abordagem escolhida foi um **Copiloto de Vendas com IA**.

Diferente de um chatbot tradicional, o copiloto não conversa diretamente com o cliente final. Ele responde para o vendedor, orientando como conduzir o atendimento.

A resposta da IA segue sempre este formato:

```md
🧠 ANÁLISE DA SITUAÇÃO
Explica o que o cliente está pedindo, qual é a dúvida, objeção ou oportunidade de venda.

💬 RESPOSTA SUGERIDA (Copie e Cole)
Mensagem pronta para o vendedor adaptar ou enviar ao cliente.

🚀 PRÓXIMA AÇÃO
Sugestão do próximo passo comercial, como perguntar algo, oferecer um produto complementar ou verificar uma informação.
```

Esse formato foi escolhido para deixar a resposta mais prática, organizada e fácil de usar em uma situação real de atendimento.

---

## 📚 Base de Conhecimento Utilizada

Para melhorar as respostas da IA, o projeto utiliza uma base de conhecimento organizada em arquivos separados.

A base contém informações sobre produtos, dúvidas frequentes e objeções comuns dos clientes.

```txt
knowledge/
├── produtos.md
├── faq.md
└── objecoes.md
```

### `knowledge/produtos.md`

Arquivo com o catálogo fictício da DB Games.

Ele reúne consoles atuais, consoles retrô, portáteis, jogos, periféricos, acessórios, itens de decoração e colecionáveis oficiais.

Também contém uma regra importante de escopo: a DB Games **não vende computadores, notebooks, placas de vídeo, peças de hardware ou montagem de PC gamer**.

### `knowledge/faq.md`

Arquivo com respostas para perguntas frequentes, como:

* formas de pagamento;
* desconto no Pix;
* parcelamento no cartão;
* envio para todo o Brasil;
* garantia de consoles novos;
* garantia de consoles usados;
* trocas e devoluções;
* avaliação de usados como parte de pagamento.

### `knowledge/objecoes.md`

Arquivo com argumentos para ajudar o vendedor a lidar com objeções, como:

* “Por que comprar um console físico se posso usar emulador?”
* “Console antigo funciona em TV moderna?”
* “Produto usado tem garantia?”
* “Essa action figure é original?”
* “Vocês vendem placa de vídeo?”
* “Vale a pena comprar jogo físico hoje em dia?”

---

## 🗂️ Estrutura do Repositório

```txt
copiloto-gamer-retro/
│
├── README.md
│
├── knowledge/
│   ├── faq.md
│   ├── objecoes.md
│   └── produtos.md
│
└── prompts/
    └── copiloto.txt
```

### Descrição dos arquivos

| Arquivo                 | Descrição                                                                           |
| ----------------------- | ----------------------------------------------------------------------------------- |
| `README.md`             | Documentação principal do projeto.                                                  |
| `prompts/copiloto.txt`  | Prompt principal do copiloto, com persona, regras de negócio e formato de resposta. |
| `knowledge/produtos.md` | Catálogo fictício de produtos da DB Games.                                          |
| `knowledge/faq.md`      | Perguntas frequentes sobre pagamento, frete, garantia e trocas.                     |
| `knowledge/objecoes.md` | Guia de apoio para lidar com dúvidas e objeções dos clientes.                       |

---

## ⚙️ Regras Principais da Solução

O copiloto foi criado com algumas regras importantes:

1. **Apoiar o vendedor humano**, não substituir o atendimento.
2. **Responder sempre no formato definido**, com análise, resposta sugerida e próxima ação.
3. **Não inventar produtos, preços, garantias ou prazos.**
4. **Usar a base de conhecimento como referência.**
5. **Recusar educadamente pedidos fora do escopo da loja.**
6. **Sugerir produtos alternativos quando algo não estiver disponível.**
7. **Estimular vendas complementares**, como acessórios, jogos, cases, películas, luminárias e colecionáveis.
8. **Manter linguagem clara, comercial e natural para WhatsApp.**

---

## 🚫 Limitação de Escopo

A DB Games **não trabalha com informática geral**.

Portanto, o copiloto deve orientar o vendedor a recusar educadamente pedidos como:

* placa de vídeo;
* RTX 4060;
* processador;
* memória RAM;
* notebook gamer;
* montagem de PC gamer;
* peças de computador.

Nesses casos, a IA deve redirecionar o atendimento para produtos que fazem parte do catálogo da loja, como PlayStation 5, Xbox Series X, Nintendo Switch ou consoles retrô.

---

## 💬 Exemplo de Uso

### Situação

O vendedor recebeu a seguinte mensagem de um cliente:

```txt
Opa, vocês trabalham com placa de vídeo? Estou precisando de uma RTX 4060 ou queria saber se vocês montam PC gamer completo.
```

### Resposta esperada do copiloto

```md
🧠 ANÁLISE DA SITUAÇÃO

O cliente está pedindo um produto fora do escopo da loja. A DB Games não vende peças de computador, placas de vídeo ou montagem de PC gamer. A melhor abordagem é responder com educação, explicar o foco da loja e redirecionar o interesse para consoles de alto desempenho.

💬 RESPOSTA SUGERIDA (Copie e Cole)

Opa, tudo bem? Nós não trabalhamos com placas de vídeo, peças de computador ou montagem de PC gamer. Nosso foco aqui na DB Games é em consoles de videogame, jogos, acessórios e colecionáveis oficiais.

Mas se a ideia é jogar com ótimo desempenho e sem a dor de cabeça de montar um PC, temos opções como PlayStation 5 e Xbox Series X. Quer que eu te mande os modelos disponíveis?

🚀 PRÓXIMA AÇÃO

Oferecer os consoles atuais disponíveis e destacar pontos como praticidade, garantia, formas de pagamento e jogos compatíveis.
```

---

## 🧪 Mensagens de Teste

Algumas mensagens usadas para testar o comportamento do copiloto:

```txt
1. O cliente perguntou se o Game Boy Advance SP vale a pena, já que ele pode jogar em um emulador de celular de graça. O que eu respondo?

2. Um cliente quer saber se o Super Nintendo funciona em TV moderna. Como explico isso?

3. O cliente perguntou se a action figure é original e se a caixa está perfeita. O que eu falo?

4. Um cliente quer comprar um Nintendo Switch Lite e perguntou se dá para incluir case e película. Como conduzo?

5. O cliente perguntou se vendemos RTX 4060 ou montamos PC gamer. Como respondo sem perder a venda?

6. Um cliente quer uma action figure específica que não está no catálogo. Como ofereço alternativas?

7. O cliente perguntou qual é a garantia de um PS2 usado. O que devo responder?

8. O cliente quer saber se o jogo físico de PS2 é original e se roda em console bloqueado.

9. Um cliente quer montar uma estante gamer com luminárias e quadros. Como posso sugerir produtos?

10. O cliente quer comprar console, jogo e item decorativo no mesmo pedido. Como posso montar uma oferta complementar?
```

---

## ✅ Como o Projeto Atende ao Desafio

| Diretriz do desafio                           | Como foi atendida                                                |
| --------------------------------------------- | ---------------------------------------------------------------- |
| Escolher um tema                              | Loja gamer fictícia chamada DB Games.                            |
| Definir usuário principal                     | Vendedores e atendentes comerciais.                              |
| Resolver um problema de vendas ou atendimento | Apoia respostas, objeções, dúvidas e próximos passos comerciais. |
| Escolher uma abordagem                        | Copiloto de Vendas com IA.                                       |
| Usar base de conhecimento                     | Arquivos de produtos, FAQ e objeções.                            |
| Mostrar exemplo gerado                        | Exemplo de atendimento com cliente pedindo placa de vídeo.       |
| Indicar melhorias futuras                     | Seção com possíveis evoluções do projeto.                        |

---

## 🚀 Possíveis Melhorias Futuras

Algumas melhorias que poderiam ser adicionadas em versões futuras:

* criar uma interface simples para o vendedor consultar o copiloto;
* conectar o copiloto a um estoque real;
* atualizar preços automaticamente;
* criar filtros por categoria de produto;
* registrar as dúvidas mais comuns dos clientes;
* gerar relatórios de objeções frequentes;
* adaptar respostas para diferentes canais, como WhatsApp, Instagram e balcão;
* transformar o projeto em um chatbot interno para a equipe comercial.

---

## 🏁 Conclusão

Este projeto mostra como a IA pode ser usada de forma simples e prática para apoiar vendas e atendimento ao cliente.

A solução não busca substituir o vendedor, mas ajudá-lo a responder melhor, manter o atendimento organizado e conduzir a conversa com mais clareza.

Com um prompt bem estruturado e uma base de conhecimento organizada, o copiloto consegue sugerir respostas mais úteis, contextualizadas e alinhadas ao negócio.
