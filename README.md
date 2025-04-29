# python-machine-learning-dash
 
# Sobre os dados

Os dados importados foram obtidos do [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/45/heart+disease). Esses dados foram doados em 1988 e provêm dos resultados clínicos e de testes não invasivos realizados em pacientes submetidos a exames na Cleveland Clinic em Cleveland (Ohio), no Instituto Húngaro de Cardiologia em Budapeste, em um Centro Médico em Long Beach (Califórnia), e também em pacientes de Hospitais universitários em Zurique e Basel (Suíça).

Inicialmente, o conjunto de dados continha 76 variáveis, mas todas as análises realizadas concentram-se no uso de um subconjunto de 14 delas. Vale destacar que, até o momento, o banco de dados da _Cleveland Clinic_ é o único utilizado por pesquisadores de aprendizado de máquina. As análises realizadas com esse banco de dados tem como objetivo distinguir a presença da doença cardíaca (valores 1, 2, 3, 4) da sua ausência (valor 0).

No nosso projeto, substituímos valores maiores que zero por 1, o que significa que um valor de 1 indica a presença de doença cardíaca, enquanto um valor de 0 indica a ausência da mesma.

Saber quais são as _features_ do dataset é fundamental para compreender mais a fundo as informações e os padrões que podem indicar a presença ou ausência de doença cardíaca. Que tal entender mais a fundo as _features_ deste conjunto de dados?

A seguir temos uma explicação sobre cada uma delas:

- `age`: Idade em anos;
- `sex`: Sexo biológico (0 = feminino, 1 = masculino);
- `cp`: Tipo de dor no peito relatada pelo paciente (1= angina típica, 2 = angina atípica, 3 = não angina, 4 = angina assintomática);
    
    > **Angina** é uma condição médica caracterizada por dor ou desconforto no peito.
    
- `trestbps`: Pressão arterial medida em repouso ;
    
    > **Pressão arterial** é a força que o sangue exerce contra as paredes das artérias à medida que é bombeado pelo coração para o resto do corpo.
    
- `chol`: Nível de colesterol no sangue em miligramas por decilitro (mg/dl);
- `fbs`: Nível de glicose no sangue em jejum, indicando se está abaixo de 120 mg/dl ou acima de 120 mg/dl (0 = abaixo, 1 = acima);
- `restecg`: Resultados do eletrocardiograma em repouso (0 = normal, 1 = anormalidade de onda ST-T, 2 = hipertrofia ventricular esquerda);
    
    > O **eletrocardiograma**, frequentemente abreviado como ECG, é um exame médico que registra a atividade elétrica do coração ao longo do tempo. Quando os resultados da eletrocardiografia (ECG) em repouso são considerados "normais", isso significa que a atividade elétrica do coração está dentro dos padrões regulares. Já quando existe anormalidade da onda ST-T pode ser um indicativo de algum tipo de irregularidade na função cardíaca. Por fim, na hipertrofia ventricular esquerda temos um aumento do tamanho do músculo cardíaco no lado esquerdo do coração.
    
- `thalach`: Frequência cardíaca máxima alcançada durante um teste de esforço físico;
- `exang`: Indica se houve angina (dor no peito) induzida por exercício ou não (0 = sim, 1 = não);
- `oldpeak`: Medida da depressão do segmento ST induzida pelo exercício em relação ao repouso;
    
    > Vamos imaginar o coração como uma bomba, e o eletrocardiograma (ECG) como um gráfico que mostra como essa bomba está funcionando. O **segmento ST** é como um intervalo na leitura desse gráfico que nos diz quando o coração está relaxando depois de bater. Agora, se durante esse relaxamento, o gráfico mostra uma parte chamada "segmento ST" mais baixa do que o normal, é como se o coração dissesse "Ei, não estou recebendo sangue suficiente aqui!" Essa baixa no gráfico é chamada de **depressão do segmento ST**.
    
- `slope`: Inclinação do segmento ST no pico do exercício (1 = inclinado para cima, 2 = plano, 3 = inclinado para baixo);
    
    > Esses resultados estão basicamente descrevendo como o coração responde ao esforço físico, olhando para um gráfico do batimento cardíaco e vendo se ele sobe, fica nivelado ou desce nesse momento específico do exercício.
    
- `ca`: Número de vasos sanguíneos principais coloridos durante o procedimento de fluoroscopia;
    
    > A fluoroscopia dos vasos sanguíneos é um exame de imagem para visualizar em tempo real o fluxo de sangue nos vasos sanguíneos.
    
- `thal`: Resultado do exame de cintilografia com tálio (3 = normal, 6 = defeito fixo, 7 = defeito reversível);
    
    > A cintilografia com tálio é um procedimento de imagem que emprega uma substância radioativa para analisar o fluxo sanguíneo e a função cardíaca. Esse exame é valioso para detectar regiões do coração que apresentam comprometimento ou baixa viabilidade.