Na página Vehicles, uma chamada à api, carrega os veículos cadastrados para o state da página. 
O veículos no state são filtrados de acordo com as opções de filtros configuradas pelo usuário; 
após esse primeiro filtro, os resultados são filtrados novamente pelo pelas palavras de busca que o usuário preenche no campo buscar. 
Os resultados são então mostrados para o usuário na forma de Cards. 

Criei dois Providers com o useContext hook para manter um estado global consistente, 
sem precisar passar props para componentes filhos que estejam “no fundo” da pilha de chamada. 

O primeiro provider é o de formulário, ele é utilizado para manter os dados que o usuário preenche ao interagir com o formulário, 
é ele também responsável por manter os dados enquanto o usuário edita um veículo já cadastrado. 

O segundo provider é o de filtro, ele é utilizado para que o usuário preencha os filtros de busca que ele deseja. 
As opções disponíveis de filtro são inferidas dos veículos que existem no state da página Vehicles, assim, 
o usuário não poderá selecionar, por exemplo, uma marca de carro a qual não exista em nenhum carro cadastrado no banco de dados. 

### Installation
O repositório front end pode ser encontrado aqui https://github.com/caio2525/corelab_FrontEnd

O repositório back end pode ser encontrado aqui https://github.com/caio2525/corelab_Back_End

Um vídeo com explicações pode ser encontrado aqui https://clipchamp.com/watch/boa6FjiKfK6

1. Clone o repositório

2. Instale as dependências
   ```sh
   npm install
   ```
3. Tenha certeza que o backend já esteja rodando

4. Rode o comando
    ```sh
   npm start
   ```
Abra [http://localhost:3000](http://localhost:3000) com seu navegador para ver o resultado.
