# Todo List

## ✅ Objetivo

Desenvolver uma aplicação TO-DO List utilizando Java e Spring Boot.

## 💻 Tecnologias e Ferramentas

![Spring Boot](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

## Steps to Setup

### 1. Clone the repository

> git clone https://github.com/BrenoCidade/todolist

### 2. Start the application via Maven package or Start it using Spring Boot Application as default:
 `todolist/src/main/java/com/brenocidade/todolist/user/UserController.java`

### 3. The App will start running at http://localhost:8080/

___

## Explore HTTP Methods:

| Http Methods(users)     | URL                                                 |
| ----------------------- | --------------------------------------------------- |
| GET                     | http://localhost:8080/users/                        |
| POST                    | http://localhost:8080/users/                        |

| Http Methods(tasks)    | URL                                                 |
| ----------------------- | --------------------------------------------------- |
| GET                     | http://localhost:8080/tasks                         |
| POST                    | http://localhost:8080/tasks                         |
| PUT                     | http://localhost:8080/tasks/{id}                    |

You can use them using a REST client such as Apidog, Postman, Insomnia, etc.

Be careful to use the correct Id and remove the `{userId}`. For example: 
> Put - http://localhost:8080/users/5321daa0-b26f-4540-a7a5-91c84ff70777

## How use Http Methods(users):

`GET` : http://localhost:8080/users

Getting all users from the Database.

Body Return:

```Json
[
    {
        "id": "90a4e416-f761-4791-bc5b-dbd28513b85f",
        "username": "userteste",
        "password": "$2a$12$RLR1qXhKlsNEYTGo.JWxDuCmyYB7ZIZAhO88QI0lbiExXgtOoo0kK",
        "name": "User Teste",
        "createdAt": "2024-06-28T12:06:55.654851"
    }
]
```
___

`POST` : http://localhost:8080/users/ 

Creating one user within the Database.

Body: 

```Json
{
    "name": "User Teste",
    "username": "userteste",
    "password": "1234"
}
```
___

## How use Http Methods(tasks):

`GET` : http://localhost:8080/tasks/  

Getting all tasks from the Database.

Body Return:

```Json
[
    {
        "id": "0a7b79ce-ad66-4795-9b97-ffb46399475f",
        "title": "Gravacao de aula3",
        "description": "Tarefa para gravar aula",
        "startAt": "2024-08-02T21:30:00",
        "endAt": "2024-08-02T22:30:00",
        "priority": "Alta",
        "idUser": "90a4e416-f761-4791-bc5b-dbd28513b85f",
        "createdAt": "2024-06-28T12:34:03.424383"
    }
]
```
___

`POST` : http://localhost:8080/tasks/   

Creating one task within the Database.

Body: 

```Json
{
    "title": "Gravacao de aula3",
    "description": "Tarefa para gravar aula",
    "startAt": "2024-08-02T21:30",
    "endAt": "2024-08-02T22:30",
    "priority": "Alta"
}
```
___

`PUT/{id}` : http://localhost:8080/tasks/0a7b79ce-ad66-4795-9b97-ffb463994342

Updating a task by Id.

Body: 

```Json
{
    "title": "Titulo novo",
    "priority": "Media"
}
```
___


## 🤝 Collaborators

We thank the following people who have contributed to this project:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/BrenoCidade" title="GitHub">
        <img src="https://avatars.githubusercontent.com/u/121961040" width="100px;" alt=""/><br>
        <sub>
          <b>Breno Cidade</b>
        </sub>
      </a>
    </td>
  </tr>
</table>
