# Machine Learning For Good
Repositório integrado ao Civis para predição de Regular Givings em churn.


## Como funciona ?

Através da tabela 'dados org' treinamos um modelo MLP para identificar Regular Givings que possuam as caracteristicas dos doadores que estão propensos a não contribuir nos próximos meses, quando for implementado o caminho será:

- Execução programada Diária/Semanal/Mensal do script
- Resultado nas regular givings com sua categoria de churn
- Registro nos Objetos do Salesforce com essa informação
- Elaboração de listas para jornadas de retenção
- Acompanhamento da Evolução dos cancelamentos
- Relatoria de resultados


## O que pode ser melhorado ?

Agora que temos um protótipo é necessário acompanhar os resultados e identificar dados que sejam relevantes para o treino do modelo, como uma primeira tentativa usamos apenas algumas informações relevantes, porem podemos adicionar ao longo do projeto outras informações que estejam relacionadas de forma direta e relevante ao cancelamentos das pessoas que já foram engajadas.
