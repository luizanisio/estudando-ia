# estudando-ia

## Consolidando algumas dicas e estudos de IA e ML

Resolvi consolidar alguns resultados de estudos realizados com o uso de elasticsearch e python para facilitar o trabalho de quem está iniciando nessa área. Esse não é um trabalho acadêmico e não visa esgotar todo o assunto.

Alguns tópicos abordados aqui com exemplos funcionais e dicas de como evoluí-los e usá-los no dia-a-dia. Estão mais próximos de receitas do tipo pegar, adaptar e usar.
 
- <b> Elasticsearch</b> utilizando o elasticsearch na classificação de documentos, identificação de fluxos de trabalho e textos relacionados (dicas, faq, etc). Uma forma simples, sustentável e rápida de implementar um classificador com bons resultados, sem a necessidade de geração e atualização de modelos. https://github.com/luizanisio/classificador_elastic

- <b> Elasticsearch + sklearn (comparação e resumo de documentos)</b> utilizando o elasticsearch para comparar dois ou mais documentos, e para sumarizar documentos encontrando as sentenças relevantes do mesmo, sem precisar guardar os documentos no elastic. Incluí também um exemplo de comparação de documentos com shingles, stop words, tfidf etc em <b>3 linhas</b> usando o <b>Sklearn</b>. A principal diferença é que o sklearn usa os próprios documentos para a identificação dos termos relevantes (<i>neste exemplo</i>), e com o elastic usamos os algoritmos do elastic para calcular os termos relevantes em seu conjunto de documentos e usando os analisadores que criarmos (com seu stemmer, stopword, sinônimos etc). Da mesma forma podemos calcular os pesos de cada sentença de um documento e criar um algoritmo de resumo por extração. https://github.com/luizanisio/comparador_elastic
 
- <b>Em elaboração</b> <i>(estou organizando os códigos)</i>: algumas dicas e exemplos práticos de treinamento em redes neurais utilizando a biblioteca Spacy (criando modelos de extração de entidades, dependência entre elas e classificação de textos). O Spacy é uma ferramenta poderosa e relativamente simples de usar. https://github.com/luizanisio/spacy_treino
 
- <b>Em breve</b>: esse código ainda não está completo, mas estou elaborando um workflow de treinamento para o Spacy, permitindo a geração, atualização e deploy de modelos gerados no Spacy. A ideia é ter uma interface de marcação de entidades, dependências e classificações, tendo um motor atualizando os modelos e permitindo testes e deploy dos mesmos de forma automatizada. Se eu achar um antes de fazer, vou postar aqui.
 
- Criando vetores de palavras (<b>word2vec</b>) com <b>Gensim</b> para tratar similaridade textual em domínios específicos com o uso do <b>Spacy</b>. Incluindo a visualização do universo de termos usando o <b>tensorboard</b>. Ainda é possível gerar um dicionário de sinônimos para ser usado no elasticsearch. https://github.com/luizanisio/word2vec_spacy
 
## Links interessantes:

- Elasticsearch: https://www.elastic.co/
- NLP com redes neurais: Spacy: https://spacy.io/  https://github.com/explosion/spaCy
- sklearn: http://scikit-learn.org
- IDE python: PyCharm https://www.jetbrains.com/pycharm/
- Cliente git: https://www.gitkraken.com

### Docker:
  - conteinerizar os serviços python: https://hub.docker.com/_/python/
  - conteinerizar o elasticsearch e kibana: https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html

## Cursos gratuitos básicos:

- <b>Curso Inteligência Artificial Fundamentos</b>: https://www.datascienceacademy.com.br/course?courseid=inteligencia-artificial-fundamentos
- <b>Python Fundamentos para Análise de Dados</b>: https://www.datascienceacademy.com.br/course?courseid=python-fundamentos
- <b>Bootcamp for KNIME Analytics Platform</b> (teoria e ferramenta) https://www.udemy.com/course/knime-bootcamp/
- <b>Advanced NLP with spaCy</b>: https://course.spacy.io/

## Cursos acessíveis básicos:
- <b>Curso Machine Learning para todos</b> (com Weka): https://www.udemy.com/share/101F6mAkUccFlbRHo=/
- <b>End to End Data Science Practicum with Knime</b> (teoria e ferramenta) https://www.udemy.com/course/datascience-knime/learn/

## Cursos gratuitos mais específicos/avançados:
- <b>Aprendizagem Automática</b> (Stanford University):  https://www.coursera.org/learn/machine-learning/home/welcome
- <b>MemSQL developer</b>: https://training.memsql.com/courses/memsql-65-developer-sp-training

## Agradecimentos
- Estou consolidando aqui estudos na área de IA/ML e cada código ou exemplo tem a participação direta ou indireta dos meus colegas de trabalho Rodrigo López, Thiago Gomes e Amilar Martins, que me apresentaram ao mundo IA. E de grandes profissionais como o Ricardo Bernardes e João Bosco que contribuem diariamente para o meu aprendizado em códigos e soluções diversas. E o meu padrinho Prof. Dr. Luciano Vieira Lima que desde sempre me dá dicas importantes em todas as áreas técnicas ou não.
