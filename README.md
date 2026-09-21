# Gerador de Certificados — Cacheadu's Academy

Gera os certificados do workshop **Técnicas Exclusivas e Inovadoras para Soltura de Cachos**
a partir de uma lista de nomes, em PNG individual, PNG em lote ou PDF com a turma inteira.

É um único arquivo HTML. Não precisa de instalação, servidor, internet nem conta em lugar
nenhum: a arte e as fontes estão embutidas no próprio arquivo e tudo é desenhado no navegador.

## Como usar

1. Abra o arquivo `Gerador de Certificados — Cacheadu's Academy.html` (duplo clique já basta).
2. Cole os nomes das alunas na caixa da esquerda, um por linha.
3. Clique em um nome da lista para conferir como ele fica no certificado.
4. Baixe:
   - **Baixar PNG desta aluna** — só a que está selecionada;
   - **Baixar PNG de todas** — um PNG por aluna, em sequência;
   - **Imprimir / salvar PDF com todas** — na janela de impressão escolha
     *Salvar como PDF*, papel A4 e **margens zero**.

## Trocando a arte

O certificado não está preso à arte que vem embutida.

- **Adicionar arte…** abre o seletor de arquivos (aceita vários de uma vez), ou você pode
  arrastar imagens direto sobre a área da prévia. PNG, JPG e WEBP.
- As artes viram miniaturas clicáveis. A arte padrão é sempre a primeira e não pode ser
  removida; as demais têm um **×** no canto.
- **Arraste sobre a arte** para posicionar o nome. As setas do teclado ajustam de 1 em 1
  pixel, e com Shift de 10 em 10.
- Os controles abaixo da prévia ajustam tamanho, largura da linha, alinhamento, cor,
  maiúsculas e negrito. As guias tracejadas mostram onde o nome cai e **nunca saem** no
  PNG nem no PDF.
- A página de impressão vira retrato sozinha se a arte for vertical.

A posição do nome é guardada em frações da arte, não em pixels, então a mesma calibragem
vale para imagens de qualquer tamanho. Cada arte guarda a sua, e o navegador lembra dela
nas próximas vezes.

## Privacidade

Nada sai do navegador: não há requisição de rede, upload nem telemetria. Os nomes das
alunas **não são gravados** em lugar nenhum — a lista começa vazia a cada abertura, de
propósito. O navegador só guarda o posicionamento do nome em cada arte.

## Tipografia

Roboto Condensed (pesos 400 e 500) embutida como WOFF2, em dois subconjuntos: `latin` e
`latin-ext` — este último é o que traz Ç, Ã, É e companhia.

## Estrutura

| Arquivo | O que é |
| --- | --- |
| `Gerador de Certificados — Cacheadu's Academy.html` | o gerador inteiro: arte, fontes, interface e código |
| `index.html` | redireciona para o arquivo acima, para o link do site ficar curto |
