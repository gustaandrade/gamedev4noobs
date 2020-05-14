# Heightmap

Já mostramos como afetar diretamente nosso mapa e como esculpir, mas, como exatamente funciona os filtros?

## Filter Level Strengths

Os níveis de filtro são baseados no tamanho total do mapa(ou área) dividido pelo nível em questão, por exemplo:

Considerando um mapa 2017x2017, o step 1 seria 2017 / 2, afetando diretamente o bloco em questão.

Com isso, quer dizer que este filtro afeta 4 blocos de tamanho 1008x1008.

Agora, o step 2 seria 2017 / 4, então estamos considerando 16 blocos por 504x504, e assim sucessivamente.

Levando isso em consideração:

- Quando quisermos modelar diretamente o mapa em seu contexto geral, utilizamos steps menores.

- Quando quisermos afetar partes individualmente utilizamos níveis maiores,

- Níveis intermediários quando quisermos afetar pequenas áreas de relevo.

[Próxima Seção](./7-Estradas.md)