# 📊 Simulador de Controle de Investimentos

## 💡 O que é este app?

Este projeto é um **simulador de controle de investimentos** desenvolvido em **planilha do Excel**, voltado para investidores que desejam planejar aportes mensais, estimar patrimônio acumulado e projetar dividendos ao longo dos anos.

---

## ❓ Perguntas respondidas pelo simulador

- Quanto investir por mês?
- Por quantos anos investir?
- Qual será o patrimônio acumulado ao final?
- Quais os dividendos mensais esperados?

---

## ⚙️ Funcionalidades técnicas implementadas

### 📁 Importação de Imagem
- Importação de banner (exemplo), com ajuste para imagem **fixa** e **não redimensionável** conforme alterações na planilha.

### 📈 Tabela: Investimento Mensal
- Criação da tabela que responde as perguntas de negócio.
- Fórmulas de cálculo com a função `VF` (Valor Futuro).
- Células de fórmula bloqueadas para evitar edições acidentais.
- Indicadores de:
  - Patrimônio acumulado.
  - Dividendos mensais.

### ⚙️ Tabela: Configurações
- Campos preenchidos pelo usuário:
  - Salário mensal.
  - Rendimento mensal da carteira.
- Cálculo automático de **sugestão de investimento de 30% do salário**.

### 🔮 Tabela: Cenários de Investimento
- Projeções de patrimônio e dividendos em **2, 5, 10, 20 e 30 anos**.
- Células referenciadas e **congeladas** para evitar perda de dados.
- **Nomenclatura das células** para facilitar leitura e fórmulas:
  - `salario` → aporte mensal  
  - `anos` → quantidade de anos  
  - `taxa_mensal` → rendimento mensal  
  - `patrimonio` → valor acumulado  
  - `soma` → dividendos mensais

### 👤 Tabela: Perfil do Investidor
- Perfis: **Conservador**, **Moderado** e **Agressivo**.
- Simulação de como R$500,00 seriam distribuídos entre TIPOS de FII com base no perfil.
- Uso de **tabela auxiliar** (na Planilha 2) com percentuais predefinidos por perfil.

### 📌 Dinâmica de Cálculo
- Seleção dinâmica do perfil com **lista suspensa**.
- Fórmula dinâmica com concatenação:  
  `=perfil&"-"&TIPO_FII`
- Utilização da função `PROCV` para buscar os percentuais com base no perfil selecionado.
- Ao alterar o perfil, a distribuição de R$500,00 se ajusta automaticamente conforme as regras do perfil.

### 📊 Gráfico de Pizza
- Inserção de gráfico com os percentuais simulados para visualização da alocação dos R$500,00 em diferentes TIPOS de FII.

---

## 📎 Considerações finais

Este simulador foi criado com foco em clareza, organização e facilidade de uso, permitindo ao investidor visualizar cenários realistas de evolução patrimonial e distribuição de investimentos com base no seu perfil.

---
