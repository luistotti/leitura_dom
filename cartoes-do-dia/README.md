# Cartões do Dia

Site simples para aplicar em casa, todos os dias, sessões curtas no estilo **Glenn Doman**: cartões de palavras, cartões de pontos, bits de inteligência, pares, frases, minilivros e uma atividade de sons e letras. A criança ganha estrelas por participar, sobe de nível e completa um álbum de figurinhas.

É um arquivo só (`index.html`), sem instalação e sem servidor. Funciona no celular, no tablet e no computador.

> Material de apoio, não oficial. Não é publicação da IAHP nem de Glenn Doman. Baseado em um dossiê de revisão crítica do método. O uso recomendado é como **complemento lúdico**: para alfabetizar de verdade, a criança também precisa aprender a relação entre letras e sons, ler histórias e escrever.

## Como usar

1. Abra o `index.html` no navegador, ou publique no GitHub Pages (veja abaixo).
2. Na tela **Brincar**, toque em **Começar sessão**.
3. Mostre cada cartão e diga a palavra com naturalidade. Toque no cartão para avançar.
4. No fim, marque como estava o interesse da criança. Isso entra no diário da aba **Pais**.

Não é preciso configurar nada. O site já vem com 3 sessões por dia e o perfil de pré-escola (3 a 5 anos). Para mudar, use a aba **Pais**.

## Rotina automática

O site monta cada dia sozinho. A aba **Rotina** mostra os próximos 14 dias.

| Conteúdo | Como avança |
|---|---|
| Palavras | O primeiro conjunto (5 cartões) fica 5 dias. Depois sai 1 palavra e entra 1 nova por dia. |
| Pontos | Quantidades de 1 a 5 no começo, avançando no mesmo ritmo até 20. Depois, contas com pontos. |
| Bits de inteligência | 5 dias por categoria. Nomes nos 2 primeiros dias, fatos a partir do 3º. |
| Leitura | Dias 1 a 10: palavras soltas. Dia 11: pares. Dia 21: frases. Dia 31: minilivros. |
| Sons (6 anos ou mais) | Uma sequência "uma letra muda tudo" por dia. A última palavra é inédita. |

O "dia da rotina" só avança nos dias em que há pelo menos uma sessão. Se pular um dia, nenhum conteúdo é perdido.

### Temas das palavras (ordem da rotina)

| # | Tema | Dias (aprox.) | Palavras |
|---|---|---|---|
| 1 | Família | 1 a 10 | MAMÃE, PAPAI, IRMÃO, IRMÃ, AMIGO, AMIGA, BEBÊ, PROFESSOR, MENINA, MENINO |
| 2 | Animais | 11 a 20 | GATO, CACHORRO, PATO, CAVALO, LEÃO, MACACO, JACARÉ, TARTARUGA, BALEIA, CAPIVARA |
| 3 | Brinquedos | 21 a 30 | BOLA, LIVRO, DADO, BLOCO, LÁPIS, PAPEL, BONECO, CORDA, CARRINHO, MOCHILA |
| 4 | Natureza | 31 a 40 | SOL, LUA, CHUVA, VENTO, NUVEM, ÁRVORE, FLOR, RIO, PEDRA, FOLHA |
| 5 | Espaço | 41 a 50 | FOGUETE, ESTRELA, PLANETA, SATURNO, MARTE, COMETA, ASTRONAUTA, UNIVERSO, GALÁXIA, TERRA |
| 6 | Dinossauros | 51 a 60 | DINOSSAURO, FÓSSIL, ROCHA, OSSO, OVO, PRESA, GARRA, CIÊNCIA, MUSEU, ESPÉCIE |
| 7 | Casa | 61 a 70 | CASA, PORTA, JANELA, MESA, CADEIRA, SOFÁ, CAMA, BANHO, COZINHA, QUARTO |
| 8 | Comidas | 71 a 80 | PÃO, LEITE, MAÇÃ, BANANA, UVA, ARROZ, FEIJÃO, QUEIJO, BOLO, CENOURA |
| 9 | Ações | 81 a 90 | PULAR, CORRER, LER, CANTAR, DORMIR, ABRIR, FECHAR, PINTAR, OLHAR, BRINCAR |
| 10 | Cores e jeitos | 91 a 100 | AZUL, VERDE, ROXO, AMARELO, VERMELHO, GRANDE, PEQUENO, RÁPIDO, LENTO, MACIO |

Depois do dia 100 a lista recomeça. As outras listas (pares, frases, minilivros, bits e sons) estão em [`docs/conteudo.md`](docs/conteudo.md).

## Estrelas e figurinhas

As estrelas vêm de **participar**, nunca de acertar. O método pede brincadeira, não prova.

| Ação | Estrelas |
|---|---|
| Cada atividade da sessão | +3 |
| Terminar a sessão, mesmo parando antes | +5 |
| Cumprir a meta do dia | +10 |
| Cada 7 dias seguidos | +15 |

Uma figurinha nova a cada 40 estrelas (40 figurinhas no álbum). Sessões além da meta do dia não valem estrelas, para não incentivar exageros.

## Área dos pais

- Calendário das últimas 5 semanas e diário das sessões com o interesse (1 a 5).
- Registro das palavras novas lidas na atividade de sons (sozinho, com ajuda, ainda não).
- Ajustes: idade, sessões por dia, cartões por conjunto, etapa de leitura (automática ou fixa), maiúsculas ou minúsculas, letra vermelha ou preta, avanço automático e voz.
- Guia rápido do método, quando parar e sinais de que vale avançar.

## Onde ficam os dados

O progresso fica salvo no **navegador do aparelho** (`localStorage`). Cada aparelho tem seu próprio progresso, e limpar os dados do navegador apaga tudo. Use sempre o mesmo aparelho e o mesmo navegador.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (por exemplo, `cartoes-do-dia`).
2. Envie os arquivos desta pasta:

   ```bash
   git init
   git add .
   git commit -m "Cartões do Dia"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/cartoes-do-dia.git
   git push -u origin main
   ```

3. No repositório, vá em **Settings → Pages**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)` e salve.
4. Em um ou dois minutos o site fica em `https://SEU-USUARIO.github.io/cartoes-do-dia/`.

Dica: no celular, abra esse endereço e use **Adicionar à tela inicial** para abrir como um app.

## Cuidados (do dossiê)

- Sessões curtas e alegres. Pare antes de a criança cansar.
- Não transforme em prova nem teste na frente da família.
- Irritação, recusa repetida ou cansaço: reduza, troque de atividade ou dê uma pausa.
- Nunca troque sono, brincadeira livre ou escola por mais sessões.
- Leia histórias todos os dias, fora dos cartões.
- Dificuldade persistente com letras e sons: converse com a escola e procure um profissional.
