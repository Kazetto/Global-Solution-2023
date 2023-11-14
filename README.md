# Global-Solution-2023---Hapvida FIAP Global Solution 2023
Desafio: Detecção de anomalias em imagens médicas usando
CNN
Contexto:
A detecção automática de anomalias em imagens médicas, como raios-X, ressonância magnética e tomografias, é uma área de pesquisa em rápido crescimento no campo da saúde. A detecção de anomalias pode auxiliar os médicos a identificar doenças como tumores, fraturas
ou outras condições médicas anormais de maneira mais rápida e precisa.

Objetivo:
Desenvolver um modelo de CNN que possa detectar anomalias em um conjunto de dados de imagens médicas. O modelo deve ser capaz de identificar e localizar a anomalia na imagem,
bem como classificar o tipo de anomalia (se possível).

Coleta de Dados:
O dataset ChestX-ray compreende 112.120 imagens de raios-X de vista frontal de 30.805 pacientes, com quatorze rótulos de doenças identificados por mineração de texto (onde cada imagem pode ter múltiplos rótulos), extraídos dos respectivos relatórios radiológicos usando processamento de linguagem natural. As quatorze patologias torácicas comuns incluem Atelectasia, Consolidação, Infiltração, Pneumotórax, Edema, Enfisema, Fibrose,Efusão, Pneumonia, Espessamento Pleural, Cardiomegalia, Nódulo, Massa e Hérnia , o que
é uma extensão dos 8 padrões de doenças comuns listados no artigo do CVPR2017. Observe que os relatórios de radiologia originais (associados a esses estudos de raios-X do tórax) não são destinados a ser compartilhados publicamente por muitos motivos. Espera-se que os
rótulos de doenças extraídos por mineração de texto tenham precisão superior a 90%. Encontre mais detalhes e desempenho de referência de modelos treinados baseados em 14 rótulos de doenças em nosso artigo no arXiv: 1705.02315.
Os dados de imagens médicas são publicos e estão disponibilizados em:
https://nihcc.app.box.com/v/ChestXray-NIHCC.
Licença e atribuição md2pdf - Markdown to PDF 13/11/2023, 10:02

Não há restrições de uso das imagens de radiografia de tórax da NIH. No entanto, o conjunto de dados tem os seguintes requisitos de atribuição:
Forneça um link para o site de download da NIH: https://nihcc.app.box.com/v/ChestXrayNIHCC
Inclua uma citação no documento CVPR 2017:

Desenvolvimento:
Como referência para o inicio do seu desenvolvimento, utlize o o repositório: https://github.com/anshuak100/NIH-Chest-X-ray-Dataset/tree/master (esse repositório serve apenas como guia inicial e não deve ser utilizado como parte da sua solução.) Siga as etapas de desenvolvimento como as ferramentas do KDD-Process ou CRISP-DM , isso inclui as etapas:

Entendimento de negocio: conhecer o conjunto de dados e o problema a ser resolvido;
pre-processamento: Tecnicas de normalização dentre outras;

Arquitetura da CNN: Desenvolver uma arquitetura CNN adequada para a detecção de
anomalias. Começar com arquiteturas famosas, como VGG, ResNet, etc., e adaptá-las
conforme necessário;

Treinamento: Dividir o conjunto de dados em treinamento, validação e teste. Treinar o
modelo usando o conjunto de treinamento e validar usando o conjunto de validação.
Implementar técnicas de regularização, como dropout ou regularização L2, para evitar
overfitting.

Avaliação: Avaliar o modelo no conjunto de teste usando métricas como precisão, recall, F1-score e AUC-ROC. Visualizar as regiões da imagem onde a rede está mais atenta (usando técnicas como mapas de calor).
Otimização: Otimizar o modelo com base nos resultados da avaliação. Experimentar diferentes arquiteturas, hiperparâmetros ou técnicas de pré-processamento para melhorar
o desempenho.

Apresentação:
Video técnico de no máximo 3min. Apresentação detalhando sua abordagem, resultados e conclusões.
Considerar as implicações éticas do uso de IA em diagnósticos médicos.
Compartilhar os desafios enfrentados e como eles foram superados.
Rubrica de Avaliação:
Compreensão do Problema (20%): Capacidade de entender e articular o problema de
detecção de anomalias em imagens médicas.
Qualidade do Modelo (30%): Eficácia do modelo em termos de métricas escolhidas
(precisão, sensibilidade, etc.).
Inovação e Criatividade (20%): Habilidade em experimentar com diferentes arquiteturas e
técnicas.
Documentação e Apresentação (15%): Qualidade da documentação (jupyter notebook)do
projeto e a clareza na apresentação dos resultados.
Reflexão Crítica (15%): Capacidade de refletir criticamente sobre os resultados, limitações e
possíveis melhorias do modelo.
Dicas:
Usar as bibliotecas TensorFlow, Keras para implementar a CNN;
Explorar o site: https://datasets.activeloop.ai/docs/ml/datasets/nih-chest-x-ray-dataset/
Experimentar técnicas como transfer Learning, usando modelos pré-treinados e
adaptando-os para esta tarefa específica.
