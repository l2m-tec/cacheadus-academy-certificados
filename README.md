# Gerador de Certificados — Cacheadu's Academy

Gera certificados a partir de uma lista de nomes, em PNG individual, PNG em lote ou PDF
com a turma inteira. O curso, a foto da modelo, os termos escritos e o restante do texto
são editáveis direto na página — não é preciso abrir editor de imagem nenhum.

É um único arquivo HTML. Não precisa de instalação, servidor, internet nem conta em lugar
nenhum: a arte original, as fontes e o modelo editável estão embutidos no próprio arquivo,
e tudo é desenhado no navegador.

## Como usar

1. Abra o arquivo `Gerador de Certificados — Cacheadu's Academy.html` (duplo clique já basta).
2. Cole os nomes das alunas na caixa da esquerda, um por linha.
3. Clique em um nome da lista para conferir como ele fica no certificado.
4. Baixe:
   - **Baixar PNG desta aluna** — só a que está selecionada;
   - **Baixar PNG de todas** — um PNG por aluna, em sequência;
   - **Imprimir / salvar PDF com todas** — na janela de impressão escolha
     *Salvar como PDF*, papel A4 e **margens zero**.

## Editando o conteúdo do certificado

O modelo que vem selecionado por padrão — **Modelo editável** — reproduz a arte original
em camadas: cada informação (nome do curso, foto, termos, assinaturas, régua, logo) é um
elemento independente, não um desenho fixo.

- **Clique em qualquer elemento do certificado** na prévia para selecioná-lo — ou use os
  botões (chips) logo abaixo da prévia, um por elemento.
- Com um elemento selecionado, o formulário abaixo mostra o que dá para editar: o texto
  (nome do curso, termos, nomes da instrutora), o tamanho, a cor, o alinhamento e, para a
  foto/logo/rubrica, um botão para trocar a imagem.
- **Arraste o elemento** na prévia para reposicioná-lo; as setas do teclado ajustam de 1
  em 1 pixel (Shift = 10 em 10).
- Cada elemento pode ser **ocultado** sem apagar o conteúdo, com a caixa "Ocultar este
  elemento".
- **Restaurar modelo** devolve o certificado ao layout original, se algo sair do lugar.

Os termos escritos aceitam qualquer texto e quebram linha automaticamente dentro da
largura definida. O nome do curso é um bloco de linhas independentes — dá para adicionar,
remover ou reescrever cada linha.

### Usando uma arte pronta em vez do modelo editável

Também dá para usar uma imagem pronta como certificado (sem camadas separadas), do jeito
que a versão anterior deste gerador trabalhava. O arquivo já vem com duas artes prontas
embutidas, além do modelo editável:

- **Arte original (pronta)** — o layout roxo original da Cacheadu's Academy.
- **Cacheadu's Cosmetics (pronta)** — um segundo design, com a foto, o logo, o texto do
  curso e as duas assinaturas de educadora já desenhados na própria arte; só o nome da
  aluna é escrito por cima, centralizado na linha em branco.

E dá para adicionar as suas próprias:

- **Adicionar arte pronta…** abre o seletor de arquivos (aceita vários de uma vez), ou
  arraste imagens direto sobre a área da prévia. PNG, JPG e WEBP.
- Nesse caso só o **nome da aluna** fica editável por cima da imagem; o resto do
  certificado já vem pronto na arte.
- Todas as artes (as embutidas e as que você adicionar) e o modelo editável aparecem
  juntos como miniaturas clicáveis, para alternar entre eles.

A posição de cada elemento é guardada nas coordenadas da própria arte usada naquele
modelo, então trocar de modelo não bagunça as posições dos outros. O navegador lembra do
que foi editado (textos, posições, imagens trocadas) para a próxima abertura.

## Privacidade

Nada sai do navegador: não há requisição de rede, upload nem telemetria. Os nomes das
alunas **não são gravados** em lugar nenhum — a lista começa vazia a cada abertura, de
propósito. O navegador guarda apenas as edições feitas no modelo (textos, posições e
imagens trocadas), para elas não se perderem entre uma sessão e outra.

## Tipografia

Roboto Condensed (pesos 400 e 500) embutida como WOFF2, em dois subconjuntos: `latin` e
`latin-ext` — este último é o que traz Ç, Ã, É e companhia.

## Estrutura

| Arquivo | O que é |
| --- | --- |
| `Gerador de Certificados — Cacheadu's Academy.html` | o gerador inteiro: arte, fontes, interface e código |
| `index.html` | redireciona para o arquivo acima, para o link do site ficar curto |
