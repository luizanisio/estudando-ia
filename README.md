# estudando-ia

## Consolidando algumas dicas e estudos de IA e ML

Resolvi consolidar alguns resultados de estudos realizados com o uso de elasticsearch e python e ferramentas/framework de IA/ML para facilitar o trabalho de quem está iniciando nessa área. Esse não é um trabalho acadêmico e não visa esgotar todo o assunto, é um espaço de compartilhamento de conhecimento adquirido. <br>
Divirta-se!<br>
Coloquei o ano na referência de alguns conteúdos para refletir a linha de tempo.
- Mais abaixo listo alguns [links interessantes](#links-interessantes) e links para [cursos](#cursos-gratuitos-b%C3%A1sicos) para uma trilha de aprendizagem. Também uma [explicação rápida](#o-que-voc%C3%AA-pode-encontrar-por-aqui) dos códigos disponibilizados nesse repositório.

### 💡 Minha pequena reflexão sobre aprendizado de máquina vs humano: 
 - 🖥️ A máquina identifica padrões para responder a uma nova informação com dados usados no treino e sugere respostas prováveis com base nos dados selecionados por `humanos` para esse treinamento. Sua capacidade de aprendizado é limitada aos padrões identificados nos dados selecionados para o treino, e que precisam ser atualizados de tempos em tempos com dados de qualidade, exigindo esforço humano para isso. É uma ótima opção para tarefas simples e repetitivas. <i>A máquina não se cansa de fazer a mesma coisa da mesma forma indefinidamente.</i>
 - :bust_in_silhouette: Humanos identificam padrões para responder a uma nova experiência ao comparar as informações disponíveis com uma rica e complexa bagagem  `cultural`, `pessoal` e `profissional` através da sua estrutura `filogenética`, podendo buscar e interpretar novas fontes de informação e acrescentá-las quase em tempo real à sua experiência de vida, permitindo sugerir respostas mais adequadas aos novos contextos. <i>Sua capacidade de aprendizado é praticamente ilimitada</i>, o limite é o tempo e o desgaste biológico no processo de aprendizado. 
 - :point_right: O objetivo dos projetos de IA é liberar humanos de tarefas repetitivas, simples e que exigem pouca inteligência na sua execução, para que esses humanos possa realizar melhor tarefas realmente inteligentes.
 > :warning: É sempre bom lembrar que a máquina não aprende como o ser humano aprende, ela não vai absorver conhecimento dos dados, textos ou imagens apresentados no treinamento e nem vai interpretá-los com base na sua bagagem filogenética, ontogenética e cultura. O que vemos como resultado de vários cálculos assemelha-se em alguns momentos ao que vemos como resultado de comportamentos humanos encobertos (processos intelectuais, pensamentos, interpretações, etc), o que faz parecer que existem processos humanos acontecendo também dentro da máquina. Colocando uma máquina em um "corpo humanóide", logo surge a ideia que as máquinas estão muito próximas de se tornarem humanas. :no_entry_sign: 
 
## O que você pode encontrar por aqui: 
Alguns tópicos abordados aqui com exemplos funcionais e dicas de como evoluí-los e usá-los no dia-a-dia. Estão mais próximos de receitas do tipo pegar, analisar, adaptar e usar. Sempre que possível estarei incluindo novos estudos e códigos funcionais.

- `2023` <b> [Doc2VecRapido](https://github.com/luizanisio/Doc2VecRapido)</b> e <b>[Doc2BertRapido](https://github.com/luizanisio/Doc2VecRapido)</b> são duas classes que simplificam o uso de um modelo Doc2Vec ou de um modelo BERT. Doc2VecRapido é mais simples que o [Doc2VecFacil](https://github.com/luizanisio/Doc2VecFacil) no treinamento de um modelo personalizado (com poucas configurações), usando o framework [`Gensim 4.0.1`](https://radimrehurek.com/gensim/). Também está disponível a classe `AgrupamentoRapido` que permite clusterizar documentos vetorizados com qualquer modelo e gerar uma planilha excel com o resultado. Veja também algumas dicas de como realizar pesquisa vetorial no [SingleStore/MemSQL](https://github.com/luizanisio/Doc2VecFacil/blob/main/docs/readme_dicas.md) e no [ElasticSearch](https://github.com/luizanisio/PesquisaElasticFacil/blob/main/docs/ElasticQueries.md).

- `2022` <b> Serviço-OCR </b> ainda em um formato de prova de conceito (nov/2022). O objetivo do [Servico-OCR](https://github.com/luizanisio/Servico-OCR) é analisar a qualidade, performance e regiões identificadas pelo Tesseract para permitir a criação de regras ou treinamento de modelos para identificar regiões como Citações, Estampas laterais, Cabeçalho e Rodapé. A identificação pode ser feita por regras simples, como margens em páginas padronizadas (A4, Carta, Legal etc). E também pode ser identificado por repetições de textos em áreas específicas, como cabeçalhos e rodapés. Quando as regras não forem suficientes, pode-se treinar um modelo com as informações mapeadas pela extração, como número de palavras, bordas, margens, posicionamento, dentre outras.

- `2021` <b> Elasticsearch fácil e preciso</b> como transformar o uso de operadores simples e de proximidade de termos em consultas robustas do ElasticSearch sem que o usuário precise conhecer a sintaxe do ElasticSearch, veja aqui: [PesquisaElasticFacil](https://github.com/luizanisio/PesquisaElasticFacil) , incluindo dicas de queries mais robustas do ElasticSearch para proximidade de termos, veja aqui: [ElasticQueries](https://github.com/luizanisio/PesquisaElasticFacil/blob/main/docs/ElasticQueries.md).

- `2022` <b> Doc2Vec criando um modelo de forma fácil</b> um componente que simplifica a criação de um vocab para treinamento do Doc2Vec e a curadoria do modelo em treinamento usando o framework [`Gensim 4.0.1`](https://radimrehurek.com/gensim/), veja aqui: [Doc2VecFacil](https://github.com/luizanisio/Doc2VecFacil), com alguns componentes para criar e fazer curadoria de [`ngramas`](https://github.com/luizanisio/Doc2VecFacil/blob/main/readme_ngramas.md), transformação de termos durante a tokenização, dentre outros. E algumas dicas de como realizar pesquisa vetorial no [SingleStore/MemSQL](https://github.com/luizanisio/Doc2VecFacil/blob/main/docs/readme_dicas.md) e no [ElasticSearch](https://github.com/luizanisio/PesquisaElasticFacil/blob/main/docs/ElasticQueries.md)

- `2022` <b>PesquisaTextualBR</b> um componente de pesquisa textual implementado com recursos em python puro com o uso de dicionário de sinônimos e distância entre termos pesquisados. Permite criar regras de pesquisa para rotulação de texto semelhante a um classificador multilabel só que com regras no lugar de um modelo treinado. Veja aqui [PesquisaTextualBR](https://github.com/luizanisio/PesquisaTextualBR).

- `2019` <b> Elasticsearch</b> utilizando o elasticsearch na classificação de documentos, identificação de fluxos de trabalho e textos relacionados (dicas, faq, etc). Uma forma simples, sustentável e rápida de implementar um classificador com bons resultados, sem a necessidade de geração e atualização de modelos. [Classificador Elastic](https://github.com/luizanisio/classificador_elastic). Se combinado com vetores usando o [Doc2VecFacil](https://github.com/luizanisio/Doc2VecFacil), pode trazer resultados ainda mais precisos.

- `2019` <b> Elasticsearch + sklearn (comparação e resumo de documentos)</b> utilizando o elasticsearch para comparar dois ou mais documentos, e para sumarizar documentos encontrando as sentenças relevantes do mesmo, sem precisar guardar os documentos no elastic. Incluí também um exemplo de comparação de documentos com shingles, stop words, tfidf etc em <b>3 linhas</b> usando o <b>Sklearn</b>. A principal diferença é que o sklearn usa os próprios documentos para a identificação dos termos relevantes (<i>neste exemplo</i>), e com o elastic usamos os algoritmos do elastic para calcular os termos relevantes em seu conjunto de documentos e usando os analisadores que criarmos (com seu stemmer, stopword, sinônimos etc). Da mesma forma podemos calcular os pesos de cada sentença de um documento e criar um algoritmo de resumo por extração. [Comparador Elastic](https://github.com/luizanisio/comparador_elastic) 

- `2019` Criando vetores de palavras (<b>word2vec</b>) com <b>Gensim</b> para tratar similaridade textual em domínios específicos com o uso do <b>Spacy</b>. Incluindo a visualização do universo de termos usando o <b>tensorboard</b>. Ainda é possível gerar um dicionário de sinônimos para ser usado no elasticsearch. [Word2Vec com Spacy](https://github.com/luizanisio/word2vec_spacy) 

- `2019` <b>Em elaboração</b> <i>(estou organizando os códigos)</i>: algumas dicas e exemplos práticos de treinamento em redes neurais utilizando a biblioteca Spacy (criando modelos de extração de entidades, dependência entre elas e classificação de textos). O Spacy é uma ferramenta poderosa e relativamente simples de usar. [Spacy Treino](https://github.com/luizanisio/spacy_treino) 
 
- `2019` <b>Em breve</b>: esse código ainda não está completo, mas estou elaborando um workflow de treinamento para o Spacy, permitindo a geração, atualização e deploy de modelos gerados no Spacy. A ideia é ter uma interface de marcação de entidades, dependências e classificações, tendo um motor atualizando os modelos e permitindo testes e deploy dos mesmos de forma automatizada. Se eu achar um antes de fazer, vou postar aqui.
 
## Links interessantes:
`2021` 
- NLP com redes neurais: Spacy: https://spacy.io/ - https://github.com/explosion/spaCy
- sklearn: http://scikit-learn.org
- Framework Gensim (vetorização): https://radimrehurek.com/gensim/
- Cadeia de Markov: https://en.wikipedia.org/wiki/Markov_chain
- Redes Neurais, como funsionam? [Prof Vinicius Caridá - parte 1](https://www.youtube.com/watch?v=EtnBTb0MKqs), [parte 2](https://www.youtube.com/watch?v=kgReLNhXsOI), [parte 3](https://www.youtube.com/watch?v=UHR2LIw4KMA) e [github da live](https://github.com/vfcarida/Live_Redes-Neurais)
- SVM, como funciona? [Prof Vinicius Caridá](https://www.youtube.com/watch?v=E3DRhPymT6Y)
- Elasticsearch: https://www.elastic.co/
- MemSQL / SingleStore (banco de dados vetorial NewSQL): https://www.singlestore.com/
- IDE python: [PyCharm](https://www.jetbrains.com/pycharm/), [VSCode](https://visualstudio.microsoft.com/pt-br/vs/community/)
- Cliente git: https://www.gitkraken.com

## Ferramentas 
`2020` 
- Knime (ferramenta para análise de dados e ML): https://www.knime.com/
- Python na nuvem com o Google Colaboratory: https://colab.research.google.com/
- Weka: https://en.wikipedia.org/wiki/Weka_(machine_learning)

### Docker:
`2019` 
  - conteinerizar os serviços python: https://hub.docker.com/_/python/
  - conteinerizar o elasticsearch e kibana: https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html

## Cursos gratuitos básicos:
`2021` 
- <b>Curso Inteligência Artificial Fundamentos</b>: https://www.datascienceacademy.com.br/course?courseid=inteligencia-artificial-fundamentos
- <b>Python Fundamentos para Análise de Dados</b>: https://www.datascienceacademy.com.br/course?courseid=python-fundamentos
- <b>End to End Data Science Practicum with Knime</b> (teoria e ferramenta) https://www.udemy.com/course/datascience-knime/
- <b>Advanced NLP with spaCy</b>: [spacy2](https://course.spacy.io/) e [spacy3](https://spacy.io/usage/v3/)
- <b>Introdução à ciência de dados e outros</b>: https://www.datascienceacademy.com.br/cursosgratuitos
- <b>Aprendizagem profunda (avançado)</b>: https://www.coursera.org/specializations/deep-learning
- <b>Weka</b>: https://www.udemy.com/course/machine-learning-e-deep-learning/learn/lecture/10409622?start=0#overview
- <b>Deeplizard - aprendizagem profunda com tensorflow (avançado)</b>: https://deeplizard.com/

## Cursos acessíveis básicos:
`2021` 
- <b>Curso Machine Learning para todos</b> (com Weka): https://www.udemy.com/course/machine-learning-e-deep-learning/
- <b>End to End Data Science Practicum with Knime</b> (teoria e ferramenta) https://www.udemy.com/course/datascience-knime/learn/

`2022`
- <b>Machine Learning e Data Science com Python de A a Z</b>: https://www.udemy.com/course/machine-learning-e-data-science-com-python-y/

## Cursos gratuitos mais específicos/avançados:
`2022` 
- <b>HarvardX CS50's</b> Introduction to Artificial Intelligence with Python: https://www.edx.org/course/cs50s-introduction-to-artificial-intelligence-with-python
- <b>Aprendizagem Automática</b> (Stanford University):  https://www.coursera.org/learn/machine-learning/home/welcome
- <b>SingleStore/MemSQL</b> cursos oficiais: https://training.singlestore.com/
<hr>

## Agradecimentos
- Estou consolidando aqui estudos na área de IA/ML e cada código ou exemplo tem a participação direta ou indireta dos meus colegas de trabalho Rodrigo López, Thiago Gomes e Amilar Martins, que me apresentaram ao mundo IA, e Rhodie Ferreira e Virgínia Martins que não se cansam de estudar e contribuir com todos a sua volta, tanto no âmbito profissional como pessoal. E de grandes profissionais como o Ricardo Bernardes, João Bosco e Osmar que contribuem diariamente para o meu aprendizado em códigos e soluções diversas. E o meu padrinho Prof. Dr. Luciano Vieira Lima que desde sempre me dá dicas importantes em todas as áreas técnicas ou não.
