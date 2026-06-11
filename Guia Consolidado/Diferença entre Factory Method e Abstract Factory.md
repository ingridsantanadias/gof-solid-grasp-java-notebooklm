A principal diferença entre esses dois padrões é a **abrangência** e o **foco** da criação:
---
*   **Factory Method:** Foca na criação de **um único produto**. Ele define uma interface para criar um objeto, mas deixa que as subclasses decidam qual classe concreta instanciar. É muito usado para delegar a lógica de criação para descendentes, aumentando a extensibilidade.
*   **Abstract Factory:** Foca na criação de **famílias de objetos** relacionados ou dependentes. Ele funciona como uma "fábrica de fábricas", permitindo que o cliente crie diversos produtos que devem ser usados juntos sem conhecer suas classes concretas.

---

Em resumo, enquanto o Factory Method resolve a criação de um objeto através de herança, o Abstract Factory resolve a criação de conjuntos de objetos através de composição. Vale notar que uma implementação de Abstract Factory frequentemente utiliza Factory Methods para criar seus produtos específicos.

