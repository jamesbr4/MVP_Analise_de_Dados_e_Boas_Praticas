# MVP_Analise_de_Dados_e_Boas_Praticas
Projeto MVP do MBA Ciência de Dados e Analytics PUC-Rio

<h1><b> Descrição do Problema </b></h1>

Utilizando o dataset de matérias-primas agrículas, Verificar as variaçoes de preços ao longo do tempo.
<h1><b> Perguntas do Problema </b></h1>

1) Descubra a variação normal do preço de cada matéria-prima;

2) Encontre a matéria-prima que tem o menor preço ao longo dos anos;

3) Qual matéria-prima tem a maior e menor variação de % de preço?

4) Encontre as matérias-primas com mudança drástica de preço;

5) Descobrir a faixa de preço de matérias-primas de baixo preço;
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
