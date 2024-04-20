## Como usar

O código Java consiste em três classes: `Main`, `ScrumBoard` e `Task`, que formam um sistema básico de gerenciamento de tarefas usando um quadro Scrum.

![imagem](https://github.com/AntonioNeto504/ADS_DEVOPS_ATIVIDADE1_SCRUM/assets/143558933/dfcbe605-374d-4764-91e9-f69ba29eee59)

- **Main**: Essa classe contém o método `main`, que é o ponto de entrada do programa. Ele cria uma instância de `ScrumBoard` e permite ao usuário interagir com o sistema através de um menu de opções. As opções incluem adicionar uma nova tarefa, visualizar tarefas existentes e marcar tarefas como concluídas.

- **ScrumBoard**: Essa classe representa o quadro Scrum e contém métodos para adicionar tarefas, visualizar tarefas e marcar tarefas como concluídas. Ela usa uma lista de `Task` para armazenar as tarefas.

- **Task**: Essa classe representa uma tarefa e possui atributos como descrição e estado de conclusão. Ela também possui métodos para obter e definir a descrição e o estado de conclusão da tarefa.

### Funcionamento do Programa:

1. O programa começa exibindo um menu de opções para o usuário.
2. O usuário pode escolher entre as opções de adicionar uma nova tarefa, visualizar tarefas existentes, marcar uma tarefa como concluída ou sair do programa.
3. Se o usuário escolher adicionar uma nova tarefa, ele será solicitado a digitar a descrição da tarefa. A tarefa será então adicionada ao quadro Scrum.
4. Se o usuário escolher visualizar tarefas existentes, o programa exibirá todas as tarefas atualmente no quadro Scrum.
5. Se o usuário escolher marcar uma tarefa como concluída, ele será solicitado a digitar o índice da tarefa a ser marcada. A tarefa correspondente será marcada como concluída.
6. O programa continuará exibindo o menu de opções até que o usuário escolha sair.

7. ![image](https://github.com/AntonioNeto504/ADS_DEVOPS_ATIVIDADE1_SCRUM/assets/143558933/7dcfb5b8-e1b0-4e34-9d4a-597367c75692)
## Execução do Docker

1. Certifique-se de ter o Docker instalado em seu sistema. Você pode baixá-lo e instalá-lo a partir do site oficial do Docker.
2. Abra o terminal ou prompt de comando.
3. Navegue até o diretório onde o arquivo Dockerfile está localizado, o qual deve ser o mesmo diretório onde o seu script PowerShell está localizado.
4. Execute o comando `docker build -t nome-da-imagem .`, substituindo "nome-da-imagem" pelo nome que você deseja dar à sua imagem Docker. Este comando construirá a imagem Docker usando as instruções do seu Dockerfile. Certifique-se de incluir o ponto `.` no final para indicar que o Dockerfile está no diretório atual.
5. Após a construção da imagem, você pode executar um contêiner Docker usando o comando `docker run`. Por exemplo, se você quiser executar um contêiner interativo a partir da imagem que acabou de criar, você pode usar o comando `docker run -it nome-da-imagem`.


 seu Dockerfile e seu script PowerShell estão configurados corretamente para serem executados em um contêiner Docker. Você pode precisar ajustar algumas configurações dependendo do que seu script faz e dos requisitos do seu ambiente Docker.


![Scrum](https://github.com/AntonioNeto504/Devops_Scrum/assets/143558933/ff5dc678-bbd4-45bf-9574-a952b8f5e5a7)



Obs: O docker não possui nenhuma interação para com caminhos de pasta, logo o código dara erro caso não haja a configuração de caminhos adquados para rodar num conteiner
