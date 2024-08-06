### Apresentação do Projeto

Este repositório no GitHub tem como objetivo comparar a performance entre Pandas e PySpark em uma análise de dados. Escolhemos uma questão do case de dados do Pandas e refizemos utilizando PySpark, realizando as seguintes análises:

1. **Comparação de Performance**:
   - Avaliamos qual ferramenta apresentou melhor desempenho na manipulação e análise dos dados.

2. **Comparação entre spark.sql e PySpark puro**:
   - Investigamos se há diferença de performance ao utilizar consultas SQL diretamente no Spark versus operações utilizando a API do PySpark.

3. **Otimização de Arquivos**:
   - Exploramos formas de otimizar os arquivos de dados, como o uso de diferentes formatos (Parquet, Avro, etc.) e a criação de particionamento, para melhorar a performance das operações de leitura e escrita.

### Particionamento no PySpark

Particionamento é uma técnica essencial para otimizar o desempenho em grandes volumes de dados no PySpark. Ele permite que o Spark distribua os dados de maneira mais eficiente pelos nós do cluster, melhorando a velocidade de leitura e processamento. Particionar os dados pode impactar positivamente a performance de análise de big data, pois:

- **Reduz o I/O**: Ao ler apenas as partições necessárias, o Spark reduz a quantidade de dados movimentados.
- **Aumenta o paralelismo**: Com mais partições, o Spark pode executar mais tarefas em paralelo.
- **Melhora a gestão de memória**: Dados particionados podem ser processados em pedaços menores, aliviando a carga de memória em cada nó do cluster.

### Testes e Resultados

Utilizamos um dataset maior do IMDb para testar a viabilidade do uso do PySpark em análises complexas e de grande volume. Nossos testes incluem:

- Comparação de tempos de execução entre Pandas e PySpark.
- Análise do impacto do particionamento e do uso de diferentes formatos de arquivo na performance do PySpark.
- Avaliação do desempenho ao utilizar consultas SQL versus operações PySpark nativas.

### Conclusão

Este projeto oferece uma visão abrangente sobre as vantagens e desvantagens de utilizar Pandas e PySpark para análise de dados, destacando as melhores práticas para otimização de performance em ambientes de big data. Fique à vontade para explorar os notebooks e scripts disponibilizados, e contribuir com sugestões e melhorias.

---
Para mais detalhes, acesse os notebooks e scripts neste repositório!
