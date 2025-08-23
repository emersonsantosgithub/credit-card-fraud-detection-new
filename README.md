# Sobre este conjunto de dados

## Contexto
É importante que as empresas de cartão de crédito sejam capazes de reconhecer transações fraudulentas de cartão de crédito para que os clientes não sejam cobrados por itens que não compraram.

## Conteúdo
O conjunto de dados contém transações realizadas com cartões de crédito em setembro de 2013 por titulares de cartões europeus.

Este conjunto de dados apresenta transações ocorridas em dois dias, nas quais registramos 492 fraudes de um total de 284.807 transações. O conjunto de dados é altamente desbalanceado, com a classe positiva (fraudes) representando 0,172% de todas as transações.

Contém apenas variáveis de entrada numéricas resultantes de uma transformação de ACP. Infelizmente, devido a questões de confidencialidade, não podemos fornecer as características originais e mais informações básicas sobre os dados.  

As características `V1, V2, ..., V28` são os principais componentes obtidos com ACP; as únicas características que não foram transformadas com ACP são **Tempo** e **Valor**.  

- A característica **Tempo** contém os segundos decorridos entre cada transação e a primeira transação no conjunto de dados.  
- A característica **Valor** é o valor da transação; esta característica pode ser usada para aprendizado sensível a custos dependente de exemplo.  
- A característica **Classe** é a variável de resposta e assume o valor 1 em caso de fraude e 0 em caso contrário.

Considerando a proporção de desequilíbrio de classes, recomendamos medir a precisão usando a **Área sob a Curva de Precisão-Recall (AUPRC)**. A precisão da matriz de confusão não é significativa para a classificação desbalanceada.
