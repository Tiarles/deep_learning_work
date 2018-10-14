# Trabalho Final da Disciplina de Deep Learning 1º/2018

Projeto feito na plataforma **Kaggle** e disponível em [Link](https://www.kaggle.com/tiarles/word2vec-via-gensim-lstm-prediction-via-keras/)

**Este exemplo não acompanha os datasets!**

Segundo Trabalho da disciplina. Profº Rodrigo da Silva Guerra

Objetivo: Implementar uma rede neural (tipo LSTM) utilizando um modelo treinado de palavras com análise por sintaxe (word2vec). 

Link 1: [Word2Vec Tutorial - The Skip-Gram Model](http://mccormickml.com/2016/04/19/word2vec-tutorial-the-skip-gram-model/)

Link 2: [Understanding LSTM Networks](http://colah.github.io/posts/2015-08-Understanding-LSTMs/)

## Parte 1: Word2Vec
A primeira parte do trabalho consiste em treinar um codificador Word2Vec seguindo uma das seguintes propostas:

* Opção 1: Treinar Word2Vec utilizando vocabulário na língua portuguesa, utilizando ferramenta padrão com implementação pronta, tal como gensim.
* Opção 2: Treinar Word2Vec utilizando vocabulário na língua inglesa, mas nesse caso implementando manualmente o algoritmo de treinamento utilizando uma biblioteca tal como TensorFlow.

Em ambos os casos os autores devem demonstrar resultados satisfatórios do treinamento, mostrando como o embedding criado agrupa palavras de categoria semanticamente afim, e mostrando resultados coerentes em operações do tipo rei - homem + mulher = rainha.

Para esta etapa será utilizado a **opção 1** com um dataset de notícias obtido pelo site Kaggle, da Folha de São Paulo. [Link 3](https://www.kaggle.com/marlesson/news-of-the-site-folhauol)

## Parte 2: LSTM
A segunda parte do trabalho consiste em implementar uma LSTM seguindo uma das seguintes propostas:
* Opção 1: Treinar LSTM para classificar sentimentos (ou classe de documento, ou outro tipo de classificação similar). Neste caso a rede deve ser treinada utilizando embeddings que se aproveitam do codificador Word2Vec implementado na Parte 1.
* Opção 2: Treinar LSTM para uma tarefa de predição da próxima palavra. Neste caso se treina a LSTM usando como entrada uma sequência de palavras de um texto, onde a rede neural deve prever a próxima palavra. Também neste caso a rede neural deve ser treinada utilizando os embeddings criados na Parte 1.
* Opção 3: Treinar LSTM para outra tarefa de predição, não necessariamente ligada a processamento de linguagem natural. Essa opção deve ter uma proposta elaborada em detalhe e aprovada pelo professor. Apenas propostas aprovadas serão consideradas para avaliação.

Para esta etapa será utilizado a **opção 1** com um dataset de frases do site *pensador.com* obtido e classicado pelo colega José Augusto Thomas ([Kaggle Profile](https://www.kaggle.com/gutothomas)) no site Kaggle, com frases de felicidade, ódio e tristeza. [Link 4](https://www.kaggle.com/gutothomas/phrases-about-happiness-from-pensadorcom), [Link 5](https://www.kaggle.com/gutothomas/phrases-about-hate-from-pensadorcom) e [Link 6](https://www.kaggle.com/gutothomas/phrases-about-sadness-from-pensadorcom).