O **GRASP** (*General Responsibility Assignment Software Patterns*) é um conjunto de nove princípios fundamentais para atribuir responsabilidades a classes e objetos na Programação Orientada a Objetos. Enquanto os padrões GoF focam em soluções específicas, o GRASP ajuda a decidir "quem faz o quê" no sistema.

As responsabilidades no GRASP são divididas em duas categorias principais:
*   **O que o objeto faz:** Executar ações, criar outros objetos ou coordenar atividades.
*   **O que o objeto sabe:** Conhecer seus dados privados, objetos relacionados ou coisas que pode calcular.

Os nove padrões que compõem o GRASP são:
1.  **Especialista na Informação:** Atribui a tarefa a quem tem a informação para realizá-la.
2.  **Criador:** Define quem deve ser responsável por instanciar novos objetos.
3.  **Baixo Acoplamento:** Busca manter as classes independentes para facilitar mudanças.
4.  **Alta Coesão:** Garante que uma classe foque apenas em sua responsabilidade.
5.  **Controlador:** Trata eventos do sistema e coordena operações.
6.  **Polimorfismo:** Lida com variações de comportamento baseadas no tipo do objeto.
7.  **Fabricação Pura:** Cria classes "artificiais" (que não existem no domínio) para manter a coesão.
8.  **Indireção:** Usa um objeto intermediário para mediar a comunicação e reduzir o acoplamento.
9.  **Variações Protegidas:** Protege o sistema contra mudanças externas através de interfaces estáveis.

O uso desses princípios resulta em um código mais organizado, de fácil manutenção e compreensão. 
