# projeto-semantix-ebac

### Diagnóstico Precoce de Doenças Cardíacas Utilizando Machine Learning

Este projeto se refere ao projeto do curso Profissão Cientista de Dados da <a href="https://ebaconline.com.br/" target='_blank'>EBAC</a> em parceria com a <a href='https://semantix.ai/' target='_blank'>SEMANTIX</a> e foi realizado para aplicar os conhecimentos adquiridos durante o referido curso.

O objetivo do projeto é:
<ul>
 <li>
     Encontrar uma problemática da vida real que possa ser
     solucionada através de análise de dados e machine learning.
 </li>
<li>Expor o problema encontrado e seus pontos.</li>
<li>Justificar a relevância do uso de dados para encontrar a solução.</li>
</ul>

As premissas para o projeto são:

<ul>
    <li>
        Levantar as fontes de dados públicas e não confidenciais
        para a coleta de informações.
    </li>
    <li>
        Efetuar a análise exploratória de dados levantando os
        principais pontos relevantes para a solução do problema.
    </li>
    <li>
        Construir um aprendizado de máquina ou modelo
        estátistico e avaliar através de técnicas de modelagem.
    </li>
    <li>
        Apresentar uma visualização de dados com os resultados
        obtidos.
    </li>
</ul>

Eu escolhi realizar um projeto sobre diagnóstico precoce de doenças cardíacas pois elas são uma das principais causas de morte no mundo e diagnósticos precoces e intervenções rápidas podem salvar vidas e reduzir significativamente os custos com cuidados de saúde a longo prazo. 

A utilização de análise de dados e machine learning para o diagnóstico precoce de doenças cardíacas pode melhorar significativamente a gestão de saúde, permitindo intervenções preventivas e reduzindo a morbidade e mortalidade associadas a essas doenças. 

Para esse projeto foi usada fonte de dados públicos, obtida de https://catalog.data.gov/dataset/rates-and-trends-in-heart-disease-and-stroke-mortality-among-us-adults-35-by-county-a-2000-45659 

Ela contém informações valiosas, como a localização geográfica, a fonte dos dados, a classe da doença, o tópico específico (neste caso, doenças cardiovasculares), a unidade de medida (por 100.000), e diferentes estratificações, como faixa etária, raça e sexo. Embora alguns valores estejam suprimidos, ainda é possível extrair insights significativos para o diagnóstico precoce de doenças cardíacas.

O dataset tem 20 variáveis/atributos:
  
* Year: Ano dos dados, útil para analisar tendências temporais.
* LocationDesc: Descrição da localização (ex.: nome do condado ou cidade).
* DataSource: Fonte dos dados, pode ser útil para entender a origem dos dados.
* Class: Classe das doenças (doenças cardiovasculares).
* Topic: Tópico específico das doenças (ex.: doenças cardíacas).
* Data_Value: Valor dos dados (taxa de doenças cardíacas), a variável-alvo.
* Confidence_limit_Low: Limite inferior do intervalo de confiança, útil para entender a precisão dos dados.
* Confidence_limit_High: Limite superior do intervalo de confiança.
* StratificationCategory1: Categoria de estratificação (ex.: grupo etário).
* Stratification1: Estratificação específica (ex.: idades 35-64 anos).
* StratificationCategory2: Categoria de estratificação adicional (ex.: raça).
* Stratification2: Estratificação específica adicional (ex.: indígena americano/nativo do Alasca).
* StratificationCategory3: Categoria de estratificação adicional (ex.: sexo).
* Stratification3: Estratificação específica adicional (ex.: geral).
* LocationID: ID da localização, útil para indexação e agrupamento. 
* GeographicLevel: Nível geográfico (ex.: condado, estado), pode ser derivado de LocationDesc.
* Data_Value_Unit: Unidade do valor dos dados (ex.: por 100.000), pode ser útil se houver diferentes unidades.
* Data_Value_Type: Tipo de valor dos dados (ex.: taxa ajustada por idade), pode ser útil para entender o tipo de medida.
* Data_Value_Footnote_Symbol: Símbolo de nota de rodapé do valor dos dados, pode ser descartado se não for relevante.
* Data_Value_Footnote: Nota de rodapé do valor dos dados, pode ser descartado se não for relevante.
 
 Vamos usar RandomForestClassifier para o diagnóstico precoce de doenças cardíacas.
