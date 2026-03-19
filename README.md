# 📊 Dashboard de Perfil de Investidor: Análise de Ações

Um projeto prático focado nos fundamentos de Análise de Dados e ETL (Extract, Transform, Load) utilizando planilhas. Este repositório demonstra a capacidade de limpar dados brutos, extrair métricas estatísticas e aplicar regras de negócio através de funções lógicas para automatizar a classificação de clientes.

---

## 💡 Google Sheets ou Microsoft Excel? A lógica é a mesma!
**Para os recrutadores e profissionais de tech:** Este projeto foi construído no Google Sheets, mas **todas as funções, lógicas de tratamento e sintaxes utilizadas aqui são 100% nativas e transferíveis para o Microsoft Excel**. 

A escolha do Sheets foi pela agilidade em nuvem, mas o domínio das estruturas condicionais (`SE`, `SOMA.SE`), extração de dados e estatística descritiva reflete uma habilidade universal em planilhas. Seja no ecossistema Google ou Microsoft, o motor lógico por baixo do capô é o mesmo! 🤝

---

## 🎯 Objetivo do Projeto (Fundamentos Sólidos)
Este é um projeto **fundacional (básico/intermediário)**. O objetivo não é criar integrações complexas, mas sim provar o domínio do "arroz com feijão" perfeito de um Analista de Dados: pegar uma base de dados crua (e neste caso, sintética), prepará-la e extrair inteligência dela sem depender de ferramentas visuais prontas.

### O que o Dashboard faz?
1. **Audita Operações:** Recebe o e-mail de um cliente e busca em milhares de linhas todo o seu histórico.
2. **Calcula Métricas Individuais:** Retorna automaticamente o volume financeiro total, quantidade de operações e ticket médio do cliente.
3. **Classifica o Perfil:** Baseado na quantidade de operações, um algoritmo lógico define automaticamente se o cliente tem um perfil **Agressivo, Moderado ou Conservador**.

---

## 🛠️ Habilidades e Fórmulas Aplicadas ("Under the Hood")

Para construir as páginas de Estatística e o Dashboard do Cliente, as seguintes técnicas e "códigos" de planilha foram utilizados:

### 1. Feature Engineering (Extração e Tipagem de Dados)
* Tratamento de tipagem (Moeda, Data, Texto).
* `DIA()`, `MÊS()`, `ANO()`: Decomposição da string de data para futuras análises de sazonalidade.

### 2. Estatística Descritiva Aplicada
Compreensão do comportamento geral da base de dados usando:
* `SOMA()`: Volume total faturado.
* `MÁXIMO()` e `MÍN()`: Identificação de topos históricos e picos de baixa.
* `MÉDIA()`, `MED()` (Mediana) e `MODO()` (Moda): Entendimento da distribuição de preços, isolando *outliers* na base de dados.

### 3. Condicionais e Lógica de Negócio (Consultas)
O equivalente a queries `SQL` feito com funções de agregação condicionais:
* `CONT.SE`: Para contar a frequência de operações de um e-mail específico.
* `SOMA.SE`: Para somar valores financeiros apenas quando a condição (ID do cliente) for verdadeira.
* `MÉDIA.SE`: Para estabelecer o ticket médio exato de cada operador.

### 4. Controle de Fluxo (If / Else)
* `SES` (ou `SE` aninhado): Criação do algoritmo de classificação do perfil do investidor com múltiplas condições lógicas (ex: `> 20 = Agressivo`, `>= 5 = Moderado`).

---

## 🚀 Como testar
Se você quiser ver as fórmulas em ação, sinta-se à vontade para clonar/fazer o download da planilha e digitar um dos e-mails da base na aba **Cliente** (use os tres primeiros e-mails para resultados diferentes). Os dados reagirão instantaneamente às fórmulas de agregação!
