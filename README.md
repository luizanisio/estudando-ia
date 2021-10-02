# estudando-ia

## Consolidando algumas dicas e estudos de IA e ML

Resolvi consolidar alguns resultados de estudos realizados com o uso de elasticsearch e python e ferramentas/framework de IA/ML para facilitar o trabalho de quem está iniciando nessa área. Esse não é um trabalho acadêmico e não visa esgotar todo o assunto, é um espaço de compartilhamento de conhecimento adquirido. Divirta-se!
Coloquei o ano na referência de alguns conteúdos para refletir a linha de tempo.

Alguns tópicos abordados aqui com exemplos funcionais e dicas de como evoluí-los e usá-los no dia-a-dia. Estão mais próximos de receitas do tipo pegar, adaptar e usar.

- `2021` <b> Elasticsearch fácil e preciso</b> como transformar o uso de operadores simples e de proximidade de termos em consultas robustas do ElasticSearch sem que o usuário precise conhecer a sintaxe do ElasticSearch, veja aqui: [PesquisaElasticFacil](https://github.com/luizanisio/PesquisaElasticFacil) , incluindo dicas de queries mais robustas do ElasticSearch para proximidade de termos, veja aqui: [ElasticQueries](https://github.com/luizanisio/PesquisaElasticFacil/blob/main/ElasticQueries.md)

- `2021` <b> Doc2Vec criando um modelo de forma fácil</b> um componente que simplifica a criação de um vocab para treinamento do Doc2Vev (gensim), veja aqui: [Doc2VecFacil](https://github.com/luizanisio/Doc2VecFacil) 

- `2019` <b> Elasticsearch</b> utilizando o elasticsearch na classificação de documentos, identificação de fluxos de trabalho e textos relacionados (dicas, faq, etc). Uma forma simples, sustentável e rápida de implementar um classificador com bons resultados, sem a necessidade de geração e atualização de modelos. [Classificador Elastic](https://github.com/luizanisio/classificador_elastic) 

- `2019` <b> Elasticsearch + sklearn (comparação e resumo de documentos)</b> utilizando o elasticsearch para comparar dois ou mais documentos, e para sumarizar documentos encontrando as sentenças relevantes do mesmo, sem precisar guardar os documentos no elastic. Incluí também um exemplo de comparação de documentos com shingles, stop words, tfidf etc em <b>3 linhas</b> usando o <b>Sklearn</b>. A principal diferença é que o sklearn usa os próprios documentos para a identificação dos termos relevantes (<i>neste exemplo</i>), e com o elastic usamos os algoritmos do elastic para calcular os termos relevantes em seu conjunto de documentos e usando os analisadores que criarmos (com seu stemmer, stopword, sinônimos etc). Da mesma forma podemos calcular os pesos de cada sentença de um documento e criar um algoritmo de resumo por extração. [Comparador Elastic](https://github.com/luizanisio/comparador_elastic) 
 
- `2019` <b>Em elaboração</b> <i>(estou organizando os códigos)</i>: algumas dicas e exemplos práticos de treinamento em redes neurais utilizando a biblioteca Spacy (criando modelos de extração de entidades, dependência entre elas e classificação de textos). O Spacy é uma ferramenta poderosa e relativamente simples de usar. [Spacy Treino](https://github.com/luizanisio/spacy_treino) 
 
- `2019` <b>Em breve</b>: esse código ainda não está completo, mas estou elaborando um workflow de treinamento para o Spacy, permitindo a geração, atualização e deploy de modelos gerados no Spacy. A ideia é ter uma interface de marcação de entidades, dependências e classificações, tendo um motor atualizando os modelos e permitindo testes e deploy dos mesmos de forma automatizada. Se eu achar um antes de fazer, vou postar aqui.
 
- `2019` Criando vetores de palavras (<b>word2vec</b>) com <b>Gensim</b> para tratar similaridade textual em domínios específicos com o uso do <b>Spacy</b>. Incluindo a visualização do universo de termos usando o <b>tensorboard</b>. Ainda é possível gerar um dicionário de sinônimos para ser usado no elasticsearch. [Word2Vec com Spacy](https://github.com/luizanisio/word2vec_spacy) 
 
## Links interessantes:
`2021` 
- Elasticsearch: https://www.elastic.co/
- NLP com redes neurais: Spacy: https://spacy.io/  https://github.com/explosion/spaCy
- sklearn: http://scikit-learn.org
- IDE python: PyCharm https://www.jetbrains.com/pycharm/
- Cliente git: https://www.gitkraken.com
- Framework Spacy: https://spacy.io/
- Framework Gensim (vetorização): https://radimrehurek.com/gensim/
- MemSQL / SingleStore (banco de dados vetorial NewSQL): https://www.singlestore.com/
- Cadeia de Markov: https://en.wikipedia.org/wiki/Markov_chain

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
- <b>Bootcamp for KNIME Analytics Platform</b> (teoria e ferramenta) https://www.udemy.com/course/knime-bootcamp/
- <b>Advanced NLP with spaCy</b>: https://course.spacy.io/
- <b>Introdução IA </b>: https://www.datascienceacademy.com.br/course?courseid=inteligencia-artificial-fundamentos
- <b>Spacy</b>: https://course.spacy.io/es/
- <b>Python completo</b>: https://www.datascienceacademy.com.br/course?courseid=python-fundamentos
- <b>Introdução à ciência de dados</b>: https://www.datascienceacademy.com.br/course?courseid=introduo--cincia-de-dados
- <b>Aprendizagem profunda</b>: https://www.coursera.org/specializations/deep-learning
- <b>Kmine</b>: https://www.udemy.com/course/datascience-knime/learn/lecture/13678654#overview
- <b>Weka</b>: https://www.udemy.com/course/machine-learning-e-deep-learning/learn/lecture/10409622?start=0#overview
- <b>Deeplizard - aprendizagem profunda com tensorflow</b>: https://deeplizard.com/

## Cursos acessíveis básicos:
`2021` 
- <b>Curso Machine Learning para todos</b> (com Weka): https://www.udemy.com/share/101F6mAkUccFlbRHo=/
- <b>End to End Data Science Practicum with Knime</b> (teoria e ferramenta) https://www.udemy.com/course/datascience-knime/learn/

## Cursos gratuitos mais específicos/avançados:
`2019` 
- <b>Aprendizagem Automática</b> (Stanford University):  https://www.coursera.org/learn/machine-learning/home/welcome
- <b>MemSQL developer</b>: https://training.memsql.com/courses/memsql-65-developer-sp-training
<hr>

## Agradecimentos
- Estou consolidando aqui estudos na área de IA/ML e cada código ou exemplo tem a participação direta ou indireta dos meus colegas de trabalho Rodrigo López, Thiago Gomes e Amilar Martins, que me apresentaram ao mundo IA, e Rhodie Ferreira e Virgínia Martins que não se cansam de estudar e contribuir com todos a sua volta, tanto no âmbito profissional como pessoal. E de grandes profissionais como o Ricardo Bernardes, João Bosco e Osmar que contribuem diariamente para o meu aprendizado em códigos e soluções diversas. E o meu padrinho Prof. Dr. Luciano Vieira Lima que desde sempre me dá dicas importantes em todas as áreas técnicas ou não.
