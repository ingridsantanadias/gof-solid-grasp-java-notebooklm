Os padrões de projeto são soluções catalogadas para problemas comuns no desenvolvimento de software, servindo como guias para criar sistemas mais robustos, flexíveis e de fácil manutenção. Eles são fundamentais para garantir requisitos como desempenho, facilidade na reutilização e agilidade na resolução de problemas recorrentes.

Abaixo, apresento um resumo detalhado dividido entre os padrões GoF, os princípios SOLID e os padrões GRASP.

---

### 1. Padrões GoF (Gang of Four)
Os 23 padrões originais são divididos em três grupos principais, baseados em sua finalidade:

#### **A. Padrões de Criação**
Focam no processo de **instanciação de objetos**, tornando o sistema independente de como seus objetos são criados e representados.
*   **Singleton:** Garante uma **única instância** de uma classe em toda a aplicação e fornece um ponto de acesso global. *Caso de uso:* Centralizar o gerenciamento de usuários ou conexões.
*   **Factory Method:** Define uma interface para criar um objeto, mas deixa as **subclasses decidirem** qual classe instanciar. *Vantagem:* Aumenta a extensibilidade e diminui o acoplamento.
*   **Abstract Factory:** Cria **famílias de objetos relacionados** sem especificar suas classes concretas. *Intenção:* Isolar o cliente das implementações específicas.
*   **Builder:** Separa a construção de um **objeto complexo** da sua representação, permitindo construções passo a passo. *Caso de uso:* Geração de objetos com muitas configurações opcionais, como diálogos Android.
*   **Prototype:** Cria novos objetos a partir da **clonagem (cópia)** de um protótipo existente. *Vantagem:* Otimiza a criação de instâncias com estados complexos.

#### **B. Padrões Estruturais**
Lidam com a **composição de classes e objetos** para formar estruturas maiores e mais complexas.
*   **Adapter:** Converte a interface de uma classe em outra esperada pelo cliente. *Função:* Atua como um "tradutor" para que sistemas incompatíveis trabalhem juntos.
*   **Bridge:** Desacopla uma **abstração de sua implementação** para que ambas possam variar independentemente. *Vantagem:* Evita a explosão de subclasses.
*   **Composite:** Agrupa objetos em estruturas de árvore para representar **hierarquias parte-todo**. *Intenção:* Tratar objetos individuais e composições de forma uniforme.
*   **Decorator:** Adiciona **funcionalidades dinamicamente** a um objeto sem usar herança. *Caso de uso:* Adicionar barras de rolagem a janelas de forma flexível.
*   **Facade:** Oferece uma **interface simplificada** para um conjunto complexo de classes em um subsistema. *Intenção:* Facilitar o uso e reduzir o acoplamento do cliente com o sistema.
*   **Flyweight:** Compartilha dados para suportar eficientemente um **grande número de objetos** pequenos. *Vantagem:* Redução significativa no uso de memória.
*   **Proxy:** Atua como um **substituto ou intermediário** para controlar o acesso a outro objeto. *Caso de uso:* Controle de acesso, carregamento sob demanda ou acesso a objetos remotos.

#### **C. Padrões Comportamentais**
Tratam das **interações e responsabilidades** entre objetos e como eles se comunicam.
*   **Chain of Responsibility:** Passa uma solicitação por uma corrente de objetos até que um a trate.
*   **Observer:** Define uma dependência um-para-muitos para que, quando um objeto mude de estado, todos os seus dependentes sejam **notificados automaticamente**. *Caso de uso:* Inscrições em canais (notificações).
*   **Strategy:** Define uma família de algoritmos e os torna **intercambiáveis em tempo de execução**. *Caso de uso:* Diferentes métodos de cálculo de frete.
*   **Command:** Encapsula uma solicitação como um objeto, permitindo operações de "desfazer".
*   **Iterator:** Permite acessar elementos de uma coleção sequencialmente **sem expor sua estrutura interna**.

---

### 2. Princípios SOLID
O SOLID é um acrônimo para cinco princípios que visam tornar o código mais compreensível e flexível.
*   **S - Single Responsibility (Responsabilidade Única):** Uma classe deve ter apenas **um motivo para mudar** (uma única função). *Vantagem:* Facilita testes e manutenções.
*   **O - Open-Closed (Aberto-Fechado):** Entidades devem estar **abertas para extensão, mas fechadas para modificação**. *Vantagem:* Novos recursos são adicionados via interfaces sem alterar o código estável.
*   **L - Liskov Substitution (Substituição de Liskov):** As subclasses devem ser capazes de **substituir totalmente suas classes base** sem quebrar a lógica.
*   **I - Interface Segregation (Segregação de Interface):** É melhor ter **interfaces específicas** do que uma única interface genérica "forçada". *Intenção:* Evitar que classes implementem métodos que não utilizam.
*   **D - Dependency Inversion (Inversão de Dependência):** Dependa de **abstrações e não de implementações concretas**. *Vantagem:* Desacopla módulos de alto nível dos de baixo nível.

---

### 3. Padrões GRASP
Os padrões GRASP (General Responsibility Assignment Software Patterns) focam na **atribuição de responsabilidades** a objetos e classes.
*   **Especialista na Informação:** Atribui a responsabilidade à classe que possui a informação necessária para cumpri-la.
*   **Criador:** Define quem deve ser responsável pela criação de instâncias de uma nova classe.
*   **Alta Coesão:** Garante que as responsabilidades de uma classe sejam focadas e relacionadas, facilitando a compreensão.
*   **Baixo Acoplamento:** Busca minimizar as dependências entre classes para que mudanças em uma não impactem as outras.
*   **Controlador:** Define qual objeto recebe e coordena os eventos do sistema ou casos de uso.
*   **Polimorfismo:** Trata variações de comportamento baseadas no tipo, usando operações polimórficas em vez de lógica condicional explícita.
*   **Fabricação Pura (Pure Fabrication):** Cria uma classe que não representa o domínio, mas presta um serviço para manter a alta coesão e o baixo acoplamento.
*   **Indireção:** Atribui responsabilidade a um objeto intermediário para mediar a comunicação entre outros dois.
*   **Proteção contra Variações:** Protege os elementos contra variações ou instabilidades de outros elementos, criando uma interface estável.
