# MVP_MAX_BRANDAO_ANALISE_DE_DADOS_E_BOAS_PRATICAS

Repositório dedicado ao MVP da disciplina de Análise de Dados e Boas Práticas da Pós-Graduação em Ciência de Dados e Analytics

Os acidentes de trânsito são uma das principais causas de morte entre jovens com idades entre 15 e 29 anos (OMS, 2018). No Brasil, de acordo com os dados divulgados pela Confederação Nacional do Transporte (CNT), o número de acidentes nas rodovias federais brasileiras aumentou em 1,6% em 2021 em relação a 2020, totalizando 64.452 casos. Além disso, houve um aumento de 2% no número de mortes, passando de 5.287 em 2020 para 5.391 em 2021, de acordo com os dados publicados pela Polícia Rodoviária Federal (PRF) (TRANSPORTE, CNT, 2021).

Portanto, este estudo tem como OBJETIVO mapear os acidentes de trânsito com vítimas fatais no país entre 2015 e 2025, permitindo avaliar e identificar a incidência e os possíveis fatores de risco associado ao óbitos nos sinistros. Os dados retratam em cada linha um conjunto de atributos relacionados a cada sinistro ocorrido nas rodovias federais do Brasil e registrados pela Polícia Rodoviária Federal (PRF) de 2015 a 2025. Os arquivos estão disponíveis no sítio https://dados.gov.br/dados/conjuntos-dados/sinistros-de-transito-agrupados-por-ocorrencia, que leva ao link https://drive.google.com/drive/folders/1eI64p7H7LRc-wWDnwjIdYmYbWurMbwbT. Toda análise foi realizada em python e disponibilizada no link a saegui:

LINK DO COLAB:
https://colab.research.google.com/drive/1ZXSjumlPImewzhEvIEnzg0UHwbEklJ6E?usp=sharing

Após a leitura dos 11 arquivos no formato .csv, houve um total de 851.191 sinistros (linhas) e 31 variáveis (atributos/colunas). Dessas, foram selecionadas 15 atributoas associados a cada sinistro, que foram: ano, mês, unidade federativa, dia da semana,  fase do dia, tipo de pista, classificação do acidente, tipo de acidente, consição de visibilidade, número de pessoas envolvidas, se houve óbito ou não, quantidade de feridos, número de mortos, latitude e longitude, que foram denominados como: 'ano', 'mes', 'uf', 'dia_semana_correto', 'fase_dia_correto', 'tipo_pista_correto', 'classificacao_acidente_correto', 'tipo_acidente_correto', 'visibilidade', 'pessoas', 'obito', 'feridos', 'mortos', 'latitude', 'longitude'. Elas foram associados ao objeto intitulado data_15_25.csv.

Para atingir os objetivos, foram fomuladas as seguintes hipóteses:

1. A quantidade de óbitos teve tendência positiva de acordo com o ano? Não, dado as análises realizadas através de medidas, de gráficos e de modelos, observamos um comportamento parabólico de rau 2 com concavidade positiva (concavidade para cima), indicando uma queda inicial seguida de um aumento;

2. Existe uma relação entre acidentes fatais e dia da semana? Existe forte relação entre os óbitos e os dias da semana, em especial no final de semana (sexta, sábado e domingo), que foi confirmado pelo gráfico de barras, pelo teste e pela análise de correspondência;

3. Há associação entre a condição de visibilidade e a ocorrência de óbito? Sim, segundo a análise das medidas, dos gráfico e da análise de correspondência, a visibilidade parcial tem maior incidência na ocorrência de acidentes fatais, sendo a condição boa e ruim relacionadas considerados fatores de proteção.

Além disso, foi detectada a relação com um maior risco de acidente fatal na região norte, seguida pela região nordeste. Tais fatos podem ser devido às condições estruturais das rodovias. Todas as variáveis avaliadas tiveram relação confirmadas estatisticamente ao nível de 5% de significância pelo teste qui-quadrado de Pearson. Em resumo, a ocorrência de óbito no sinistro tem relação com a fase do dia, em que plena noite e amanhecer são fatores de disco; com o dia da semana, com predominância para domingo, sábado e sexta; com a fase do dia, com a condição de visibilidade, de modo que a parcial é o fator de risco; e com o tipo de pista; em a pista simples é um fator de risco.

Tais resultados são relevantes para uma tomada de decisão mais segura para os condutores de modo que possam evitar acidentes fatais, bem como as instituições podem elaborar projetos públicos que conscientizem os condutores.
