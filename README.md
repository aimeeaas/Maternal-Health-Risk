# Esteira de Machine Learning — Maternal Health Risk

## Descrição do Projeto

Este projeto implementa uma esteira (pipeline) completa de aprendizado de máquina para um problema de classificação, utilizando o dataset [Maternal Health Risk](https://archive.ics.uci.edu/dataset/863/maternal+health+risk) da UCI Machine Learning Repository.

O objetivo é prever o nível de risco de saúde materna (baixo, médio ou alto) a partir de indicadores clínicos coletados via dispositivos IoT em hospitais e clínicas rurais de Bangladesh, como idade, pressão arterial, glicemia, temperatura corporal e frequência cardíaca.

O notebook cobre todas as etapas da esteira:
- Importação e exploração dos dados
- Estatísticas descritivas
- Transformação de coluna (codificação do alvo `RiskLevel`)
- Transformação de linha (remoção de duplicadas)
- Divisão em conjuntos de treino, validação e teste
- Treinamento de um modelo de classificação (Random Forest)
- Avaliação com matriz de confusão e acurácia
- Predição de um novo exemplo

## Vídeo de Apresentação

🎥 [Link para o vídeo no YouTube](https://youtu.be/n3jvQOg-8yk)

## Como Reproduzir

1. Clone este repositório ou baixe o arquivo `maternal_health_risk.ipynb`.
2. Abra o notebook no [Google Colab](https://colab.research.google.com/) (ou Jupyter local).
3. Execute as células em ordem, de cima para baixo (`Ambiente de execução → Executar tudo` no Colab).
4. As dependências (`ucimlrepo`, `pandas`, `scikit-learn`, `matplotlib`) são instaladas automaticamente na primeira célula.
5. Os dados são baixados diretamente da UCI Machine Learning Repository via `ucimlrepo`, não sendo necessário nenhum arquivo local.
6. Ao final da execução, o notebook exibe:
   - Estatísticas descritivas da base
   - A matriz de confusão e a acurácia do modelo no conjunto de teste
   - A predição de um exemplo de paciente

## Tecnologias Utilizadas

- Python 3
- pandas
- scikit-learn
- matplotlib
- Google Colab
