Análise de Sentimentos em Tweets com TextBlob
Descrição do Projeto
Este projeto realiza uma análise de sentimentos em tweets utilizando a biblioteca TextBlob para classificar cada tweet como Positivo ou Negativo. A análise permite obter insights sobre o sentimento geral expresso nos tweets, com métricas de desempenho e visualizações para avaliar a precisão do modelo.

Motivação
A análise de sentimentos em redes sociais é uma ferramenta valiosa para entender a opinião pública. Este projeto demonstra uma implementação básica que pode ser expandida para aplicações comerciais ou acadêmicas.

Estrutura do Projeto
NoThemeTweets.csv: Arquivo CSV com os tweets e rótulos de sentimento.
sentiment_analysis.py: Script principal que realiza a análise de sentimentos e gera as visualizações.
README.md: Documentação do projeto.
Requisitos
Bibliotecas Necessárias
Certifique-se de ter as seguintes bibliotecas instaladas:

bash
Copiar código
pip install pandas textblob scikit-learn matplotlib seaborn
Estrutura do Dataset
O dataset (NoThemeTweets.csv) deve conter:

tweet_text: Coluna com o texto do tweet.
sentiment: Coluna com o sentimento rotulado (Positivo ou Negativo).
Como Executar
Clone o Repositório:

bash
Copiar código
git clone https://github.com/seu_usuario/seu_projeto.git
cd seu_projeto
Prepare o Dataset: Coloque o arquivo NoThemeTweets.csv na pasta do projeto.

Execute o Script: Execute o script principal para realizar a análise:

bash
Copiar código
python sentiment_analysis.py
O script carregará o dataset, aplicará a análise de sentimento, calculará as métricas de avaliação e exibirá as visualizações.

Etapas do Código
1. Importação das Bibliotecas
O script utiliza as bibliotecas pandas, TextBlob, scikit-learn, matplotlib, e seaborn para processamento e visualização.

2. Carregamento e Preparação dos Dados
O dataset é carregado e processado para definir a coluna de texto e converter os rótulos de sentimento em valores numéricos.

3. Análise de Sentimentos
Uma função usa o TextBlob para classificar cada tweet como Positivo, Negativo, ou Neutro (caso a polaridade seja zero).

4. Filtragem de Dados Neutros
Somente tweets classificados como Positivos ou Negativos são incluídos na análise final.

5. Avaliação do Modelo
O desempenho do modelo é avaliado usando uma matriz de confusão e um relatório de classificação com precisão, revocação e F1-score.

6. Visualizações
O script gera:

Matriz de confusão para avaliação de desempenho.
Gráficos de contagem e histogramas para mostrar a distribuição dos sentimentos e polaridade dos tweets.
Exemplos de Resultados
Matriz de Confusão
A matriz de confusão mostra o número de classificações corretas e incorretas para cada categoria de sentimento (Positivo e Negativo).

Relatório de Classificação
O relatório de classificação exibe métricas como precisão e revocação para ajudar a entender o desempenho do modelo.

Visualizações
Distribuição dos Sentimentos Reais: Exibe a quantidade de tweets positivos e negativos no dataset.
Distribuição de Polaridade: Histograma da polaridade dos tweets, mostrando a frequência de valores positivos, negativos e neutros.
Melhorias Futuras
Classificação de Sentimentos Neutros: Implementar uma terceira categoria para classificar tweets neutros, em vez de excluí-los.
Modelos Avançados: Utilizar modelos de aprendizado profundo, como BERT, para melhorar a precisão da análise de sentimentos.
Interface de Usuário (UI): Desenvolver uma interface gráfica para que usuários possam inserir textos e visualizar a análise de sentimento em tempo real.
Contribuições
Contribuições são bem-vindas! Para contribuir:

Fork o repositório.
Crie uma nova branch para suas mudanças (git checkout -b feature-minha-melhoria).
Commit suas mudanças (git commit -m 'Adicionei nova funcionalidade').
Push para a branch (git push origin feature-minha-melhoria).
Abra um Pull Request.
