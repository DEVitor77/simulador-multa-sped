# 📊 Simulador de Multa SPED - ECD / ECF

![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Ativo-brightgreen)

> **Simulador interativo** para cálculo de multas por atraso na entrega da **ECD** (Escrituração Contábil Digital) e **ECF** (Escrituração Contábil Fiscal), com base na legislação vigente da Receita Federal.

🔗 **Acesse o simulador:** [https://devitor77.github.io/simulador-multa-sped/](https://devitor77.github.io/simulador-multa-sped/)

---

## 📌 Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Base Legal](#base-legal)
- [Funcionalidades](#funcionalidades)
- [Como Usar](#como-usar)
- [Cálculos Realizados](#cálculos-realizados)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Estrutura do Código](#estrutura-do-código)
- [Exemplos Práticos](#exemplos-práticos)
- [FAQ - Perguntas Frequentes](#faq---perguntas-frequentes)
- [Contribuição](#contribuição)
- [Licença](#licença)

---

## 🎯 Sobre o Projeto

Este simulador foi desenvolvido para auxiliar **contadores, empresários e profissionais da área fiscal** a calcular rapidamente o valor da multa por atraso na entrega das obrigações acessórias **ECD** e **ECF** do SPED (Sistema Público de Escrituração Digital).

O sistema considera as diferentes regras de cálculo para:
- ✅ **ECD** - Todos os regimes tributários
- ✅ **ECF** - Lucro Presumido
- ✅ **ECF** - Lucro Real (com e sem lucro)

### 🎯 Público-alvo
- Contadores e escritórios de contabilidade
- Empresários e gestores financeiros
- Profissionais do departamento fiscal
- Estudantes da área contábil

---

## ⚖️ Base Legal

### 📁 ECD (Escrituração Contábil Digital)

| **Legislação** | **Detalhamento** |
| :--- | :--- |
| **Lei 8.218/91, Art. 12, III** | Multa de 0,02% por dia de atraso sobre a receita bruta |
| **Lei 13.670/2018** | Nova redação dos arts. 11 e 12 da Lei 8.218/91 |
| **IN RFB 2.003/2021, Art. 11** | Aplicação das multas à ECD |
| **Limite máximo** | 1% da receita bruta do período |
| **Redução** | 50% se entregue antes de procedimento de ofício |

### 📊 ECF - Lucro Presumido

| **Legislação** | **Detalhamento** |
| :--- | :--- |
| **Lei 8.218/91, Art. 12, III** | Multa de 0,02% por dia de atraso sobre a receita bruta |
| **Limite máximo** | 1% da receita bruta do período |
| **Redução** | 50% se entregue antes de procedimento de ofício |
| **DARF** | Código 3624/2 |

### 🧾 ECF - Lucro Real

| **Legislação** | **Detalhamento** |
| :--- | :--- |
| **DL 1.598/77, Art. 8º-A, I** | Multa de 0,25% por mês sobre o lucro líquido |
| **Lei 12.973/2014** | Nova redação do art. 8º-A |
| **Limite máximo** | 10% do lucro líquido |
| **Redução** | 50% (espontâneo) a 90% (até 30 dias) |
| **Regra especial** | Se prejuízo, usa último lucro corrigido pela Selic |
| **DARF** | Código 3624/3 |

---

## ✨ Funcionalidades

| **Funcionalidade** | **Descrição** |
| :--- | :--- |
| 📁 **Simulação ECD** | Calcula multa com base na receita bruta |
| 📊 **Simulação ECF Presumido** | Mesma regra da ECD para Lucro Presumido |
| 🧾 **Simulação ECF Real** | Cálculo baseado no lucro líquido |
| ⚠️ **Simulação com Prejuízo** | Usa último lucro + correção Selic |
| 🌙 **Modo Escuro** | Alternância entre temas claro/escuro |
| 📄 **Exportar PDF** | Gera relatório completo da simulação |
| 📊 **Exportar CSV** | Baixa histórico em formato de planilha |
| 📈 **Gráfico Dinâmico** | Visualização comparativa dos resultados |
| 📋 **Histórico** | Armazena até 50 simulações |
| 🔄 **Atualização Automática** | Resultados em tempo real |
| 📱 **Responsivo** | Funciona em todos os dispositivos |

---

## 🚀 Como Usar

### 1️⃣ Acesse o simulador
Abra o link: [https://devitor77.github.io/simulador-multa-sped/](https://devitor77.github.io/simulador-multa-sped/)

### 2️⃣ Preencha os dados
Em cada módulo, insira:
- **Receita Bruta** ou **Lucro Líquido**
- **Data limite** (vencimento da obrigação)
- **Data efetiva** (data da transmissão)

### 3️⃣ Veja os resultados
O sistema calcula automaticamente:
- Dias/meses em atraso
- Multa cheia
- Limite aplicável
- Valor com desconto (50% ou 90%)

### 4️⃣ Utilize os recursos extras
- 📊 Compare resultados no gráfico
- 📋 Consulte o histórico de simulações
- 📄 Exporte PDF ou CSV
- 🌙 Alterne para modo escuro

---

## 🧮 Cálculos Realizados

### ECD e ECF (Lucro Presumido)

Multa = Receita Bruta × 0,02% × Dias de atraso
Limite = Receita Bruta × 1%
Valor a pagar = MIN(Multa, Limite)
Desconto = Valor a pagar × 50%


### ECF (Lucro Real)

Multa = Lucro Líquido × 0,25% × Meses de atraso
Limite = Lucro Líquido × 10%
Valor a pagar = MIN(Multa, Limite)
Desconto 50% = Valor a pagar × 50%
Desconto 90% = Valor a pagar × 10% (se ≤ 30 dias)


### ECF (Lucro Real com Prejuízo)

Lucro corrigido = Último lucro × (1 + Taxa Selic)
Multa = Lucro corrigido × 0,25% × Meses de atraso


---

## 🛠️ Tecnologias Utilizadas

| **Tecnologia** | **Finalidade** |
| :--- | :--- |
| **HTML5** | Estrutura do site |
| **CSS3** | Estilização e responsividade |
| **JavaScript (Vanilla)** | Lógica de cálculo e interatividade |
| **Chart.js** | Geração de gráficos |
| **html2canvas** | Exportação para PDF |
| **GitHub Pages** | Hospedagem gratuita |

---

## 📁 Estrutura do Código
📦 simulador-multa-sped/
├── 📄 index.html # Código principal (HTML + CSS + JS)
├── 📄 README.md # Documentação do projeto
└── 📄 LICENSE # Licença MIT (opcional)


---

## 📋 Exemplos Práticos

### Exemplo 1: ECD com Receita Bruta de R$ 100.000

| **Dados** | **Valor** |
| :--- | :--- |
| Receita Bruta | R$ 100.000,00 |
| Data Limite | 30/06/2026 |
| Data Efetiva | 13/08/2026 |
| Dias em atraso | 44 dias |

**Resultado:**
- Multa cheia: R$ 880,00
- Limite (1%): R$ 1.000,00
- **Valor a pagar: R$ 880,00**
- **Com desconto 50%: R$ 440,00**

---

### Exemplo 2: ECF Real com Lucro de R$ 100.000

| **Dados** | **Valor** |
| :--- | :--- |
| Lucro Líquido | R$ 100.000,00 |
| Data Limite | 31/07/2024 |
| Data Efetiva | 31/01/2026 |
| Meses em atraso | 18 meses |

**Resultado:**
- Multa cheia: R$ 4.500,00
- Limite (10%): R$ 10.000,00
- **Valor a pagar: R$ 4.500,00**
- **Com desconto 50%: R$ 2.250,00**
- **Com desconto 90% (≤30 dias): R$ 450,00**

---

### Exemplo 3: ECF Real com Prejuízo

| **Dados** | **Valor** |
| :--- | :--- |
| Último lucro (2021) | R$ 10.000,00 |
| Taxa Selic | 15% |
| Lucro corrigido | R$ 11.500,00 |
| Meses em atraso | 18 meses |

**Resultado:**
- Multa cheia: R$ 517,50
- **Valor a pagar: R$ 517,50**
- **Com desconto 50%: R$ 258,75**

---

## ❓ FAQ - Perguntas Frequentes

### 1. O simulador é gratuito?
✅ Sim! Completamente gratuito e hospedado no GitHub Pages.

### 2. Preciso instalar algo?
❌ Não. Basta acessar o link pelo navegador.

### 3. Funciona no celular?
✅ Sim! O design é 100% responsivo.

### 4. Os dados são salvos?
❌ Não. O histórico é apenas local (não persiste após recarregar a página).

### 5. Posso confiar nos cálculos?
✅ Sim! O simulador segue rigorosamente a legislação vigente (Lei 8.218/91 e DL 1.598/77).

### 6. O que fazer se a receita for zero?
✅ O sistema calcula multa zero. Não há valor mínimo fixo para ECD/ECF Presumido.

### 7. Como atualizar o simulador?
🔧 Basta editar o arquivo `index.html` no GitHub e fazer commit.

### 8. Posso usar meu próprio domínio?
✅ Sim! O GitHub Pages permite configurar domínio personalizado.

### 9. O histórico fica salvo se eu fechar o navegador?
❌ Não. O histórico é armazenado apenas em memória durante a sessão.

### 10. Como exportar os resultados?
📄 Clique em "PDF" para gerar um relatório ou "CSV" para baixar uma planilha.

---

## 🤝 Contribuição

Sinta-se à vontade para contribuir com este projeto!

### Como contribuir:
1. Faça um **Fork** do projeto
2. Crie uma **Branch** para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Faça o **Commit** das alterações (`git commit -m 'Adiciona nova funcionalidade'`)
4. Faça o **Push** para a Branch (`git push origin feature/nova-funcionalidade`)
5. Abra um **Pull Request**

### Sugestões de melhorias:
- [ ] Adicionar mais regimes tributários
- [ ] Incluir calculadora de juros Selic automática
- [ ] Adicionar suporte a múltiplos idiomas
- [ ] Criar versão com persistência de dados (localStorage)
- [ ] Incluir notificações por e-mail

---

## 📄 Licença

Este projeto está sob a licença **MIT**. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

MIT License

Copyright (c) 2026 devitor77

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
...


---

## 📞 Contato

**Autor:** devitor77  
**GitHub:** [@devitor77](https://github.com/devitor77)  
**Projeto:** [Simulador de Multa SPED](https://github.com/devitor77/simulador-multa-sped)  

---

## 🙏 Agradecimentos

- **Receita Federal** - Pela disponibilização das normas e legislações
- **Comunidade contábil** - Pelo feedback e sugestões
- **Open Source** - Pelas bibliotecas utilizadas (Chart.js, html2canvas)

---

## 📌 Disclaimer

> **Este simulador tem caráter meramente informativo e educativo.** 
> 
> Os cálculos são baseados na legislação vigente, porém recomenda-se sempre consultar um profissional contábil qualificado e verificar a legislação atualizada antes de tomar qualquer decisão baseada nos resultados apresentados.

---

**⭐ Se este projeto foi útil para você, considere dar uma estrela no GitHub!**

[⬆ Voltar ao topo](#-simulador-de-multa-sped---ecd--ecf)
