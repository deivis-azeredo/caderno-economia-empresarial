## **🧪 Suíte de Testes e Validação Anti-Alucinação (NotebookLM / RAG)**

Esta matriz de testes serve para validar se o modelo está estritamente ancorado nas fontes documentais fornecidas, evitando o uso de parâmetros gerais ou alucinações.

| \# | Categoria / Tipo de Teste | Pergunta de Controle (Prompt) | Comportamento Esperado (Critério de Sucesso) | Fonte de Referência |
| :---- | :---- | :---- | :---- | :---- |
| **1** | Teste de Inexistência | *"O que as apostilas dizem sobre o impacto das criptomoedas ou do Bitcoin na economia empresarial?"* | O NotebookLM deve responder claramente que o texto não menciona criptomoedas ou Bitcoin. Se inventar dados, há alucinação. | — (Controle Geral) |
| **2** | Atribuição de Exemplos Reais | *"Quais empresas específicas são citadas como exemplos nas apostilas e em qual contexto cada uma aparece?"* | Deve citar apenas as empresas presentes no texto: Tesla, Apple, Magazine Luiza, Amazon, Natura e Itaú. | Okai |
| **3** | Definições e Comparações | *"Qual é a diferença exata entre Economia Empresarial e Economia Gerencial descrita nos documentos?"* | Indicar que a Economia Empresarial tem alcance mais amplo (setor terciário e mercados) e a Gerencial é restrita ao processo decisório. | Wikipédia |
| **4** | Citação Institucional | *"O que a Universidade de Manchester e a Universidade de Miami dizem especificamente sobre a Economia Empresarial?"* | Miami foca em recursos, bancos e mercado acionário; Manchester foca na contribuição para o bem-estar da sociedade e estrutura industrial. | Wikipédia |
| **5** | Teste Sequencial (Ciclos) | *"Quais são as 4 fases do ciclo econômico explicadas no texto e o que caracteriza a fase de Pico?"* | Fases: Expansão, Pico, Recessão e Recuperação. No Pico: máximo crescimento, demanda alta, inflação e alta de juros. | Okai |
| **6** | Lista Fechada | *"Quais são as 5 dicas de economia para empresas apresentadas na apostila da Conection Soluções?"* | Listar: 1\. Planejamento financeiro; 2\. Controle de gastos/desperdícios; 3\. Tecnologia; 4\. Outsourcing; 5\. Renegociação com fornecedores. | Conection Soluções |
| **7** | Nuance de Conceito | *"Segundo os textos, a redução de custos deve ser feita cortando funcionários? Como o texto explica a produtividade?"* | Responder que não deve ser associada a cortes. O problema no Brasil é a baixa produtividade por falta de métodos e educação básica. | Transcrição / Análise |
| **8** | Gestão de Pessoas | *"Como a gamificação e a liderança podem ajudar na economia de recursos dentro da empresa segundo a apostila?"* | Citar que a gamificação cria um desafio coletivo e que líderes devem explicar cortes e compartilhar lucros gerados via bônus. | Transcrição / Análise |
| **9** | Indicadores Econômicos | *"Quais são os principais fatores econômicos mencionados que afetam a demanda, os custos e o acesso ao crédito?"* | Mencionar: Taxas de crescimento (PIB), Inflação, Taxas de Juros, Políticas Fiscais e Taxa de Câmbio. | Strong / FGV |
| **10** | Ferramental Contábil | *"Qual ferramenta contábil é apontada no texto como fundamental para começar a analisar custos e desperdícios?"* | Indicar o DRE (Demonstrativo de Resultados do Exercício). | Transcrição / Análise |

