# ROCKETSEAT/IGNITE - PRIMEIRO DESAFIO: LISTA DO QUE FAZER
Este projeto foi concebido como primeiro desafio para o programa de aceleração IGNITE, desenvolvido pela Rockseat, e é uma lista de coisa para fazer, construída através do REACT JS, Typescript e Scss.
<b>Atenção:</b> Projeto conceito.

## Índice

  - [Visão Geral](#Visão-Geral)
  - [O desafio](#O-desafio)
  - [Screenshot](#screenshot)
- [Meu processo](#Meu-processo)
  - [Construído com](#Construído-com)
  - [O que eu aprendi](#O-que-eu-aprendi)
  - [Desenvolvimento continuado](#desenvolvimento-continuado)
  - [Recursos úteis](#recursos-uteis)
- [Autor](#Autor)



## Visão geral

### O desafio

No desafio, eu deveria criar uma aplicação para treinar o que aprendi até agora no ReactJS. Esta é uma atividade onde o principal objetivo é a concepção de uma pequena aplicação de atividades a fazer, para treinar um pouco mais sobre manipulação do estado no React.


### Screenshot

![Página com uma lista do que fazer ](https://github.com/airtonlimajr/rocketseat-ignite-chapter1-challenge1/blob/main/img/Screenshot.png)



## Meu processo

## Construído com

- REACT JS
- TYPESCRIPT
- JAVASCRIPT
- SCSS

### O que eu aprendi ...

Aprendi que, para entender o funcionamento do React é necessário ter em mente alguns conceitos fundamentais que dizem respeito a funções. Outro importante aprendizado, foi sobre a utilização do Typescript no processo de criação do aplicativo, que trouxe várias melhorias no processo do desenvolvimento, como códigos mais ordenados e 
fácil detecção de erros.

<b>#Exemplos de components/TaskList.tsx :</b>

```
export function TaskList() {
  const [tasks, setTasks] = useState<Task[]>([]);
  const [newTaskTitle, setNewTaskTitle] = useState('');

  function handleCreateNewTask() {
    if (newTaskTitle) {
      setTasks([
        ...tasks,
        {
          id: new Date().getUTCMilliseconds(),
          title: newTaskTitle,
          isComplete: false,
        }
      ]);
```
```
      setNewTaskTitle('');
    } else {
      console.log('Não é possível adicionar uma tarefa vazia.');
    }
  }

```
```
function handleRemoveTask(id: number) {
    setTasks(tasks.filter(task => task.id !== id));
  }

```




### Desenvolvimento continuado

O REACT é um ótimo recurso e acrescenta mais possibilidades no já vasto mundo do desenvolvimento web, mas vale ressaltar que apesar dos diversos benefícios que estas biblioteca pode trazer ao processo de desenvolvimento Front-end,
o domínio de comandos como YARN e entre outros,  são essenciais para uma utilizaçao mais assertiva.


### Recursos úteis

- [FAQ - Desafios](https://www.notion.so/FAQ-Desafios-ddd8fcdf2339436a816a0d9e45767664) -A documentação disponível na página, foi bastante útil para sanar dúvidas sobre GIT e testes.
- [Vídeo com a solução](https://www.youtube.com/watch?v=qFuxsmgQs4Q&t=1s) - Último recurso, utilizado para testar e descobrir porque determinadas falhas ainda aconteciam.


### Airton Lima Jr

- Linkedin - [airtonlimajr](https://www.linkedin.com/in/airtonlimajr/)
