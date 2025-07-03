# MVP_Analise_de_Dados_e_Boas_Praticas
Projeto MVP do MBA Ciência de Dados e Analytics PUC-Rio

<h1><b> Descrição do Problema </b></h1>

Utilizando o dataset de matérias-primas agrículas, Verificar as variaçoes de preços ao longo do tempo.
<h1><b> Perguntas do Problema </b></h1>

1) Descubra a variação normal do preço de cada matéria-prima;
  <br>R: Podemos observar que a maioria das matérias-primas tem % de mudança frequente ideal inferior a 5%, significando que, para a maioria dos materiais, os picos dos histogramas estão localizados nos intervalos de variação percentual abaixo de 5%. Isso sugere que a variação mensal mais comum para essas matérias-primas é relativamente baixa.
2) Encontre a matéria-prima que tem o menor preço ao longo dos anos;
  <br>R: O algodão é matéria-prima de menor preço nos últimos anos.
3) Qual matéria-prima tem a maior e menor variação de % de preço?
  <br>R: Podemos ver na linha 'max' que a 'Preço da madeira serrada macia % Variação' tem o maior valor (65.24), o que confirma a observação de que ela teve os picos de variação mais altos. O desvio padrão para 'Preço da madeira serrada macia % Variação' (5.77) também é um dos mais altos, indicando alta volatilidade.<br>
Olhando para a linha 'max', a 'Preço da madeira compensada % Variação' tem um valor máximo relativamente baixo (19.50), e seu desvio padrão (2.66) também é um dos menores, confirmando a observação de que ela teve menor variação.
4) Encontre as matérias-primas com mudança drástica de preço;
  <br>R: A mudança de preço é drástica para o preço de tora dura entre materiais de baixa faixa de preço e entre materiais de alto preço, são os preços de lã fina.
5) Descobrir a faixa de preço de matérias-primas de baixo preço;
  <br>R: O intervalo interquartil está entre Q3 e Q1 mínimo, primeiro quartil (Q1), mediana, terceiro quartil (Q3) e máximo e outliers" descreve corretamente os componentes de um box plot, que são exatamente o que usamos para entender a faixa de preço de cada matéria-prima neste caso.
<h1><b> Tipo de Problema </b></h1>

Este é um problema de classificação supervisionada.
<h1><b> Seleção de Dados </b></h1>

Este conjunto de dados é composto por preços e % de variação de preço para lã grossa, copra, algodão, lã fina, tora, madeira serrada dura, couro, compensado, borracha, lenha, madeira serrada macia e polpa de madeira.

Os dados são provenientes do Indexmundi, disponibilazado no Kaggle.
<h1><b> Atributos do dataset após tratamento dos dados</b></h1>

<table>
  <tr>
    <th>Atributos</th>
    <th>Data Type</th>
    <th>Unidade</th>
  </tr>
  <tr>
    <td>Meses </td>
    <td>object</td>
    <td>data (yyyy-mm-dd)</td>
  </tr>
  <tr>
    <td>Preço da lã grossa </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da lã grossa % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço Copra </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da Copra % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço do algodão </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço do algodão % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço de lã fina </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço de lã fina % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço da tora dura </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da tora dura % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço da madeira serrada dura </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da madeira serrada dura % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço do couro</td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço do couro % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço da madeira compensada </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da madeira compensada % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço da borracha </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da borracha % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço da lenha </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da lenha % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço da madeira serrada macia </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da madeira serrada macia % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
  <tr>
    <td>Preço da polpa de madeira </td>
    <td>float64</td>
    <td>$ (dólar)</td>
  </tr>
  <tr>
    <td>Preço da polpa de madeira % Variação </td>
    <td>float64</td>
    <td>% (percentual)</td>
  </tr>
</table>
<h1>Conclusão</h1>
Este estudo realizou uma análise exploratória abrangente do dataset de Preços de Matérias-Primas Agrícolas entre 1990 e 2020, abordando desde o pré-processamento dos dados até a visualização de tendências e relações.
<br>
Inicialmente, os dados foram carregados e submetidos a um rigoroso processo de tratamento para lidar com valores ausentes, inconsistências de formato (como vírgulas e símbolos de porcentagem) e a padronização dos nomes das colunas para português, garantindo a qualidade e a usabilidade do dataset para análises subsequentes. A etapa de pré-processamento foi crucial para transformar os dados brutos em um formato limpo e estruturado, essencial para a extração de insights confiáveis.
<br>
A análise exploratória revelou características importantes dos preços das matérias-primas. Observamos que a maioria das matérias-primas apresenta uma variação percentual mensal relativamente baixa, com os picos de frequência dos histogramas concentrados abaixo de 5%. Isso indica uma estabilidade mensal predominante nos preços para grande parte dos materiais ao longo do período estudado.
<br>
Através da análise das estatísticas descritivas e dos gráficos de série temporal, foi possível categorizar as matérias-primas em grupos de "baixo preço" (como algodão, couro e borracha) e "alto preço" (incluindo lã grossa, lã fina e polpa de madeira), identificando o algodão como a matéria-prima de menor preço médio ao longo dos anos.
<br>
A investigação da volatilidade, quantificada pelo desvio padrão e valor máximo das variações percentuais, confirmou a madeira serrada macia como a matéria-prima com os picos de variação percentual mais elevados e maior volatilidade geral, enquanto a madeira compensada demonstrou ser a menos volátil. A identificação de matérias-primas com mudanças de preço "drásticas" — notavelmente a tora dura no grupo de baixo preço e a lã fina no grupo de alto preço — ressalta a importância de analisar a volatilidade tanto em termos percentuais quanto absolutos e dentro de suas faixas de preço características.
<br>
A análise de correlação, visualizada através do mapa de calor, foi fundamental para entender as relações lineares entre os preços das diferentes matérias-primas. Foi confirmado que o preço da lã grossa e da lã fina possuem uma forte correlação positiva (aproximadamente 0.89), indicando que seus preços tendem a se mover na mesma direção. Em contraste, pares como couro e borracha apresentaram correlação muito baixa, sugerindo pouca ou nenhuma relação linear em seus movimentos de preço.
<br>
Adicionalmente, a divisão dos dados em conjuntos de treinamento e teste baseada no tempo foi implementada, uma prática essencial para a modelagem preditiva de séries temporais, garantindo que o modelo seja treinado com dados históricos e avaliado em um período futuro simulado. A padronização das features foi aplicada posteriormente para escalar os dados, preparando-os para algoritmos de machine learning sensíveis à escala, enquanto se manteve a ordem temporal crucial para a análise de séries.
<br>
Em suma, este trabalho forneceu uma análise robusta do dataset de preços de matérias-primas agrícolas, revelando padrões de variação, volatilidade, faixas de preço e correlações entre os materiais. Os insights derivados são valiosos para a compreensão do comportamento histórico desses mercados e servem como base sólida para futuras análises preditivas ou financeiras.
