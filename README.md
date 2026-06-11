# ☕ Guia de Arquitetura Java: Padrões GoF, SOLID e GRASP com NotebookLM

## 📝 Contexto e Objetivos
Este repositório foi desenvolvido como o projeto prático para o desafio de portfólio da DIO. O objetivo principal deste trabalho é aplicar o conceito de **aprendizado ativo** utilizando o Google NotebookLM como um assistente estratégico de estudos. 

O foco temático escolhido foi a fundação da engenharia de software no ecossistema **Java**:
*   **Princípios SOLID:** Regras essenciais para a saúde, manutenção e testabilidade do código.
*   **Princípios GRASP:** Modelagem mental para a atribuição correta de responsabilidades a objetos.
*   **Padrões de Projeto GoF (Gang of Four):** Soluções arquiteturais consagradas para problemas recorrentes de design.

---

## 📂 Estrutura do Repositorio
Para garantir a organização e maturidade técnica exigidas no mercado, o repositório foi estruturado da seguinte forma:

*   `./links.md/` - Pasta contendo os links e referências das fontes abertas utilizadas na curadoria de dados para alimentar o NotebookLM[cite: 1].
*   `./Prompts feitos para o NotebookLM.md/` - Histórico e documentação da engenharia de prompts aplicada durante as sessões com a IA[cite: 1].
*   `./Guia Consolidado/` - Arquivos com as respostas brutas e sínteses geradas pela ferramenta para consulta.

---

## 📚 Curadoria de Fontes
A curadoria foi feita selecionando artigos e documentações de referência sobre design orientado a objetos e Java. Os links originais das fontes que fiz upload no NotebookLM estão centralizados e descritos na pasta `/Links de base` deste repositório, garantindo uma base de dados confiável e livre de alucinações da IA.

---

## 🔬 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)
O processo de extração de conhecimento não foi linear. Na pasta `/Enhenharia de Prompts`, documentei a evolução da escrita das perguntas estratégicas, comparando abordagens generalistas com prompts direcionados que forçaram a IA a trazer resumos práticos e completos.

### 🛠️ Desafios Encontrados (Troubleshooting)
*   **Diferenciação Teórica:** O NotebookLM tendeu a trazer resumos curtos e com pouca fundamentação teórica.
---

## 🎓 Miniguia de Estudo (Resumos Próprios)

Abaixo está a consolidação do meu aprendizado prático, unindo a pesquisa guiada por IA aos meus próprios resumos sobre o tema:

### 1. Resumos Estruturados

#### **SOLID em Java**
Os princípios SOLID funcionam como o controle de qualidade do código Java. O foco principal foi entender o **Single Responsibility Principle (SRP)**, evitando classes "God" que gerenciam conexões e regras de negócio ao mesmo tempo, e o **Dependency Inversion Principle (DIP)**, garantindo que nossas classes dependam de interfaces (`java.util.List`) e nunca de implementações concretas (`ArrayList`).

#### **GRASP (Atribuição de Responsabilidades)**
Antes de sair criando padrões complexos, o GRASP dita a lógica básica de onde colocar cada comportamento. Aprendi que usando o conceito de **Information Expert (Especialista na Informação)**, o método deve ficar na classe que possui os dados para executá-lo. Isso aumenta a coesão do sistema.

#### **Padrões GoF aplicados ao Java**
Quando os princípios apontam rigidez no sistema, os padrões GoF resolvem. No ecossistema Java, destaco o uso do **Strategy** para eliminar estruturas condicionais massivas (`if/else` ou `switch`) em regras de taxas ou descontos, tornando o sistema aberto para extensões sem alterar o código que já está homologado e funcionando.

### 2. Glossário de Conceitos Aprendidos
*   **Coesão:** Grau de relacionamento entre as responsabilidades de uma classe. Em Java, buscamos classes altamente focadas (Alta Coesão).
*   **Acoplamento:** Força da dependência entre classes. Quanto menor o acoplamento, mais fácil é alterar uma classe sem quebrar o restante do sistema.
*   **Fabricação Pura (Pure Fabrication):** Uma classe criada artificialmente que não representa um objeto do mundo real do negócio, mas é necessária para manter a coesão (ex: as famosas classes `Repository` ou `Service` em frameworks Java).

### 3. Prompts Reutilizáveis para Revisão Futura
*(O histórico completo está disponível na pasta `/prompts`)*

*   **Prompt de Simulado:** `"Com base no caderno, atue como um entrevistador técnico Java. Faça 3 perguntas difíceis de nível pleno sobre como implementar o padrão Observer (GoF) em sistemas concorrentes."`
*   **Prompt de Refatoração:** `"Analise o código Java que vou colar a seguir. Identifique quais princípios do SOLID ou GRASP ele viola e reescreva-o aplicando a refatoração necessária."`

---
Projeto desenvolvido para fins educacionais e de portfólio na plataforma da [DIO](https://www.dio.me/).
