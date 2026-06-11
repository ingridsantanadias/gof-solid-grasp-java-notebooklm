A principal diferença entre esses dois padrões GRASP está em **quem** recebe a responsabilidade e **por que**.

*   **Especialista na Informação:** Atribui a responsabilidade à classe que possui a informação necessária para realizá-la. O objetivo é manter o "saber" e o "fazer" juntos, seguindo a lógica natural do domínio.
*   **Fabricação Pura (Pure Fabrication):** Cria uma classe "artificial" ou fictícia que não representa um conceito do mundo real. Ela é usada quando atribuir uma tarefa ao "Especialista" prejudicaria a **Alta Coesão** ou o **Baixo Acoplamento**.

Em resumo: o **Especialista** foca na organização lógica do negócio, enquanto a **Fabricação Pura** cria classes de serviço (como um gerador de logs ou acesso a banco) para manter o sistema tecnicamente saudável.

