# Lista de Estudantes - Aplicação em React

Este projeto é uma aplicação simples de gerenciamento de estudantes utilizando React. A aplicação permite adicionar, editar, remover e pesquisar estudantes, além de persistir os dados utilizando o `localStorage` do navegador.

## Funcionalidades

1. **Adicionar Estudante**: O usuário pode adicionar um estudante inserindo o nome e clicando no botão "Adicionar". Um nome padrão de imagem é atribuído automaticamente a cada estudante.
   
2. **Editar Estudante**: O usuário pode editar o nome de um estudante clicando no botão "Editar". Isso abrirá um prompt onde o usuário pode digitar o novo nome.

3. **Remover Estudante**: O usuário pode remover um estudante da lista clicando no botão "Remover".

4. **Pesquisar Estudante**: O usuário pode buscar estudantes pelo nome. A lista de estudantes é filtrada em tempo real conforme o que o usuário digita no campo de pesquisa.

5. **Persistência de Dados**: Os dados dos estudantes são armazenados no `localStorage`, garantindo que as informações persistam mesmo após a atualização da página ou fechamento do navegador.

## Tecnologias Utilizadas

- **React**: Biblioteca JavaScript para construção da interface de usuário.
- **CSS**: Estilização da aplicação utilizando classes do Tailwind CSS (estilos utilitários).
- **localStorage**: API de armazenamento do navegador utilizada para persistir os dados dos estudantes.

## Como Usar
1. Clone o repositório para sua máquina:

   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```

2. Acesse a pasta do projeto:
   ```bash
   cd nome-do-repositorio
    ```
3. Instale as dependências:
   ```bash
   npm install
    ```
4. Inicie o servidor de desenvolvimento:
      ```bash
   npm run dev
    ```
5. Acesse a aplicação no navegador. Geralmente estará disponível em:
      ```bash
   http://localhost:5173
    ```
## Estrutura do Código
### App.js
A aplicação é composta por um único componente funcional, App, que gerencia a lista de estudantes e as interações do usuário.

- Estado (useState):

   - students: Armazena a lista de estudantes.
   
   - searchTerm: Controla o texto inserido no campo de pesquisa.
   
   - newStudentName: Controla o nome do novo estudante a ser adicionado.

- Efeitos (useEffect):

   - Carregar estudantes: Ao carregar o componente pela primeira vez, os dados dos estudantes são carregados do localStorage.
   
   - Salvar estudantes: Sempre que a lista de estudantes for atualizada, os dados são salvos no localStorage.

### Funções:
   - addStudent: Adiciona um novo estudante à lista, gerando um ID único com o timestamp atual e atribuindo uma imagem padrão.

   - removeStudent: Remove um estudante da lista com base no ID.

   - editStudent: Permite editar o nome de um estudante, solicitando ao usuário um novo nome através de um prompt.

   - filteredStudents: Filtra a lista de estudantes com base no texto inserido no campo de pesquisa.

### index.css
Este arquivo contém as regras de estilo para a aplicação. Ele usa Tailwind CSS, um framework CSS utilitário, para facilitar a estilização.

O código está configurado para aplicar estilos em elementos como botões, inputs, listas e imagens de estudantes.

## Como Contribuir
1. Faça um fork do projeto.

2. Crie uma branch para suas alterações:
   ```bash
   git checkout -b minha-branch
    ```
3. Faça as alterações e commit:
   ```bash
   git commit -m "Descrição das mudanças"
    ```
4. Faça o push para sua branch:
   ```bash
   git push origin minha-branch
    ```
5. Envie um Pull Request para o repositório principal.

# Licença
Este projeto é de código aberto sob a licença MIT.
