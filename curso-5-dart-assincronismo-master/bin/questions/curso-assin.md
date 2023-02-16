Saber o que significa Single Thread:
    Vimos que o Dart é uma linguagem Snigle Thread, ou seja, que realiza uma tarefa por vez

Identificar o que são Isolates:
    Espaços de memória ocm loops, dedicados para realizar tarefas no computador - por exemplo, abrir uma nova tela.

Saber como funcionam os Loop de Eventos:
    Funcionalidades que buscam por tarefas na pilha de exeução do programa e individualmente fazem o processo de levar as tarefas até os espaços de memórias onde serão processadas

Compreender a importância do Assincronismo:
    Técnica que separa  tarefas que precisam de um tempo de espera, a fim de tornar eficiente a execução de tarefas rápidas, enquanto esperamos por tarefas lentas (que esperam informação de fora, lugar de onde não temos controle).

Entender o funcionamento e alterar o KakoBot:
    Vimos o código padrão do nosso projeto, e como ele funciona além de olhar passo a passo os métodos que compõem a lógica por trás do nosso bot pessoal.



Criar um objeto do tipo Future:
    Aprendemos a criar o nosso primeiro objeto do tipo Future e vimos que ele não segue as regras de ordem natural dos outros objetos.
    Normalmente, o Objeto do tipo Future precisa de um tempo para receber as informações, então o próprio Dart coloca ele no final da fila de execução de tarefas, a fim de esperar pelas informações chegarem e não atrasar objetos dependentes.


Produzir uma Função Assíncrona:
    Criamos uma função que recebe a nomenclatura de async e, dentro dela, usamos um método Future.delayed() adicionando o termo await e fomentando, assim, a ação de espera em objetos do tipo Future.

Implementar tempo de espera no KakoBot:
    Em nosso projeto, adicionamos a classe BotClock() e implementamos um método clock() que cria uma função de espera baseada em segundos. Adicionamos ao nosso KakoBot alguns segundos de espera em algumas frases de espera. Assim, criamos a simulação de que nosso KakoBot está buscando informações de um banco de dados externo! Isso foi necessário para entendermos o contexto ao qual os objetos do tipo Future estão inseridos.
