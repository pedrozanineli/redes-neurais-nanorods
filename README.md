# Predição de sínteses eficientes de um nanomaterial de ouro por meio de Redes Neurais 🧠

<p style = "text-align:justify">
Neste repositório estão os arquivos e os notebooks relacionados ao Trabalho de Conclusão de Semestre da disciplina de Redes Neurais e Algoritmos Genéticos.
    </p>

<p style = "text-align:justify">
    Os nanomateriais apresentam diversas aplicações nas mais diferentes áreas, como <em>drug delivery</em>, óptica, medicina e energia. Nesse projeto, estaremos trabalhando com <b>nanorods de ouro</b>, um nanomaterial metálico de formato de bastão, com propriedades e usos ainda mais específicos. No entanto, o processo de síntese dessas <em>nanorods</em> é um processo extremamente delicado, passando por diversas etapas e demandando bastante tempo. Assim, utilizamos redes neurais para fazer predições da síntese ideal, buscando avaliar os possíveis desempenhos com variações dos parâmetros do experimento. Para o treinamento, usamos dados experimentais de diferentes sínteses, nas quais se variaram diferentes aspectos dos reagentes e se obteve diferentes dados de Espectroscopia no Ultravioleta Visível e Infravermelho Próximo (UV-VIS-NIR).
    </p>

   

Integrantes do projeto: Pedro Zanineli, Shaian Anghinoni e Felipe Minatogau

## Arquivos e Notebooks 🗂️

📁 <b>dados</b>: são os dados coletados pelo UV-VIS-NIR de cada uma das sínteses que foram desenvolvidas.  
  
📁 <b>dados tratados</b>: dados tabelados com os valores de picos, obtidos após serem tratados nos notebooks 2.0 - obtecao dados v0 e v1.

📁 <b>figs</b>:  pasta com as imagens geradas nos notebooks.  
  
📄 <b>1 -  calculo de picos.ipynb</b>: Notebook para encontrar os valores máximos de cada pico que temos de nossos dados.

<p style = "text-align:justify">
    📄 <b>2.0 - obtencao dados v0.ipynb</b> e <b>2.1 - obtencao dados v1.ipynb</b>: Tratamento de dados de UV-VIS-NIR, no qual obtemos para cada arquivo os valores máximos de pico. Como cada dado são picos com diferentes alturas, tivemos que mudar os parâmetros para cada caso, o que foi um processo manual. Portato, quando for baixar o código em seu computador, apenas rodar todo o código não irá funcionar.
    </p>
    
<p sytle = "text-align:justify">
    📄 <b>3 -  calculo de picos.ipynb</b>: Notebook onde pegamos as <em>features</em> (rotas de síntese e os dados tabelados no excel) e os <em>targets</em> e plotamos a matriz de correlação (correlação de pearson). Nossos <em>targets</em> são os valores máximos dos picos de absorbância do UV-VIS-NIR.
    </p>
    
<p sytle = "text-align:justify">
    📄 <b>4.0 - redução de dimensionalidade (n=2).ipynb</b>: Nesse notebook, aplicamos o método de Principal Component Analysis (PCA) nos dados obtidos anteriormente para encontrar as duas features principais. Aqui, utilizamos duas componentes (n=2). No outro notebook, (📄 <b>4.1 - redução de dimensionalidade (n=3).ipynb</b>), aplicamos para n=3, porém escolhemos trabalhar com a redução de dimensionalidade com duas componentes para ter uma razão maior entre os dados e as features.
    </p>
    
<p style = "text-align:justify">
    📄 <b>5 - rede neural regressor.ipynb</b>: Nesse notebook, aplicamos todas as nossas redes neurais, como a de regressão, com classificador, e com regressor e classificador com PCA de duas componentes.
    </p>
    
<p style = "text-align:justify">
    📄 <b>6 - plot importância.ipynb</b>: Nesse notebook, calculamos e plotamos as importâncias das features.
    </p>
