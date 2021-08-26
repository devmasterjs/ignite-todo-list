# ignite-todo-list
(Rocketseat Education) - Desafio 01 - Conceitos do React

## Objetivo do desafio

Nesse desafio, é necessário editar apenas o seguinte arquivo para completar as funcionalidades da aplicação:

- [src/components/TaskList.tsx;](https://github.com/rocketseat-education/ignite-template-reactjs-conceitos-do-react/blob/main/src/components/TaskList.tsx)

### components/TaskList.tsx

Esse é o componente responsável por todas as funcionalidades da aplicação, é um componente simples, mas onde botaremos em prática várias partes da manipulação do estado.

É necessário criar as funcionalidades para as três funções presentes nesse arquivo, que são:

- **handleCreateNewTask**: Deve ser possível adicionar uma nova task no estado de `tasks`, com os campos `id` que deve ser gerado de forma aleatória, `title` que deve ser um texto e `isComplete` que deve iniciar como false.
- **handleToggleTaskCompletion:** Deve alterar o status de `isComplete` para uma task com um ID específico que é recebido por parâmetro.
- **handleRemoveTask:** Deve receber um ID por parâmetro e remover a task que contém esse ID do estado.

## Especificação dos testes

Em cada teste, tem uma breve descrição no que sua aplicação deve cumprir para que o teste passe.

Para esse desafio, temos os seguintes testes:

### Teste TaskList.spec.tsx

- **should be able to add a task**

Para que esse teste passe, é necessário que task seja criada e com isso, exibida em tela. As taks criadas devem conter os atributos seguindo o padrão da interface, que é:

```tsx
interface Task {
  id: number;
  title: string;
  isComplete: boolean;
}
```

- **should not be able to add a task with an empty title**

Para que esse teste passe, antes de criar uma nova task, é preciso validar se algo foi digitado no input e não permitir a criação da task caso o valor seja vazio, caso o valor digitado seja vazio, deve-se impedir a criação da task.

- **should be able to remove a task**

Para que esse teste passe, ao clicar no botão com ícone de uma lixeira, a task relacionada a esse botão deve ser removida do estado da aplicação, e consequentemente ser removida da tela.

- **should be able to check a task**

Para que esse teste passe, ao clicar no checkbox ao lado da task, ela deve ser marcada como concluída ou não concluída de acordo com seu estado atual, alterando seu valor de `isComplete` de `false` para `true` ou ao contrário, de `true` para `false`.

## Instalação do projeto em ambiente local

Após clocar no repositório, execute um dos comandos abaixo para instalar as dependências:

```bash
yarn install
```
ou
```bash
npm install
```

## Execução do projeto em ambiente local

Para executar a aplicação, execute um dos comandos abaixo:

```bash
yarn dev
```
ou
```bash
npm run dev
```

## Execução dos testes unitários em ambiente local

Para executar os testes unitários, execute um dos comandos abaixo:

```bash
yarn test
```
ou
```bash
npm test
```
