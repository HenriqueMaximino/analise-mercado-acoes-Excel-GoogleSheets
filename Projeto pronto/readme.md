# 🚀 Projeto Finalizado: Dashboard Perfil de Investidor

Bem-vindo à pasta do projeto finalizado! Aqui você encontra o resultado da aplicação de todo o processo de ETL (Extração, Tratamento e Carregamento) e a inteligência de negócios aplicada aos dados.

## 🌐 Acesso Rápido e Interativo (Recomendado)

A melhor forma de avaliar este projeto é "brincando" com ele na nuvem. A planilha foi configurada para ser interativa. Sinta-se à vontade para ir na aba **"cliente"**, digitar diferentes e-mails da base de dados e ver as fórmulas lógicas classificando os perfis em tempo real.

👉 **[🔗 Clique aqui para acessar e testar a Planilha no Google Sheets](https://docs.google.com/spreadsheets/d/1CKOyTNEAux66rIwxROPRC46fyktK9rcvM_q5XaRMYwo/edit?usp=sharing)**

---

## ⬇️ Instruções para Download e Teste Local

Caso você prefira baixar o arquivo físico disponibilizado nesta pasta para avaliar o código das fórmulas localmente, deixo uma recomendação importante:

⚠️ **Aconselho fortemente que você abra o arquivo importando-o de volta para o Google Sheets** (ou utilizando uma versão bem atualizada do Microsoft Excel 365). 

**Por que isso é importante?** Este projeto faz uso de funções condicionais modernas (como a função `SES` / `IFS`) para construir a lógica do Perfil de Investidor. Softwares de planilhas mais antigos ou desatualizados podem não reconhecer a sintaxe corretamente, gerando o erro `#NOME?`. No Google Sheets, a compatibilidade com essas funções avançadas é 100% garantida.

---

## 📂 O que você vai encontrar nas abas do projeto:

* **📊 mercado_acoes:** A base de dados principal, já limpa e tipada, contendo a engenharia de recursos (Feature Engineering) com a extração isolada de Dia, Mês e Ano.
* **📈 estatística:** Um painel consolidado com a estatística descritiva geral da base (Volume total, Média, Mediana para isolar *outliers*, Moda, Mínimo e Máximo).
* **🎯 cliente:** O Dashboard final que cruza as informações usando `SOMA.SE`, `CONT.SE` e `MÉDIA.SE` para retornar o relatório individual de cada investidor.
