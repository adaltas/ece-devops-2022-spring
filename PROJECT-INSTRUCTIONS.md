
# Project instructions

## Deadline

April 24, 2022

## Opportunities

1. The DevOps project is based on all of the labs passed during the course, it is allowed to use them.
2. Work on the project can be carried out only by a group of 2 students or 1.

## Submitting

* Continue working in the same GitHub repository that you used for the lab works. **Don't create any other repositories!**
* The repository must be **PRIVATE** and you must give your teacher access to it. Otherwise, if it isn't PRIVATE the grade will be reduced to 0.
* The recommended structure of the project is:   
  ```
  .github/
  iac/
    Vagrantfile
    playbooks/
  image/
  k8s/
    deployment.yaml
    service.yaml
  labs/     # If you want to backup the labs corrections
    lab2/
    lab3/
    ...
  userapi/
    src/
    test/
    conf/
    CHANGELOG.md
    package.json
    Dockerfile
    ...
  README.md
  docker-compose.yaml
  ...
  ```

## Tasks

### 1. Create a web application

Create a web application on any programming language (NodeJS, Java, Ruby, Python, etc.), storing data in a database (Redis, MongoDB, MySQL, ...) and cover it with tests of different levels.

**Are proposed:**

- a little user API application with [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) user functionality
- storage in Redis database
- tests: unit, API, configuration, connection.

**Note!** You are allowed to use the draft application located in the [courses/devops/modules/03.continuous-testing/lab](courses/devops/modules/03.continuous-testing/lab) folder, but you have to enrich it by at least completing all comment sections marked "TODO".

### 2. Apply CI/CD pipeline 

Configure and apply CI/CD (including deployment) pipeline using any platforms (GitHub Actions, GitLab CI/CD, Jenkins, Netlify, Heroku, etc.).

**Note!** If the chosen deployment platform (like Heroku) requires a subscription to make use of their database service to connect to your app, you can skip using this service. In this case, your application won't be running properly, but it must successfully display the homepage. 

### 3. Configure and provision a virtual environment and run your application using the IaC approach

1. Configure with Vagrant: 1 VM running on any Linux distribution 
2. Provision the VM with Ansible, which includes installing and running:
  - language runtime
  - database
  - your application (use [sync folders](https://www.vagrantup.com/docs/synced-folders))
  - health check of your application

### 4. Build Docker image of your application

1. Create a Docker image of your application
2. Push the image to Docker Hub

**Note!** You must [ignore](https://docs.docker.com/engine/reference/builder/#dockerignore-file) all the files and folders that do not need to be included in the image.

### 5. Make container orchestration using Docker Compose

1. Create `docker-compose.yml` file that will start your application

### 6. Make container orchestration using Kubernetes

1. Install Kubernetes cluster using Minikube
2. Create Kubernetes Manifest YAML files:
  - deployments
  - services

### 7. Document your project 

Write a sort of report in the `README.md` file which includes the following:

1. List all the work performed (briefly, describing features and bonus tasks).

2. Screenshots (pictures of your screen when you are running a web page, K8s resources, VMs, etc... Provide maximum screenshots)

> Tip. Keep screenshots in a separate folder. Ex.: see how pictures are linked in the `index.md` files of the modules.

3. Provide instructions (commands) of how to:
  - Install (or prepare environment)
  - Use (your application, run your Docker container or Docker Compose, ...)
  - Test (your application)
  
4. All the necessary links with the platforms and tools integrated:
  - Heroku
  - Docker Hub
  - ...
  
5. Author

6. Other additional info that you want to include...

> **Note!** Use the correct Markdown syntax to keep your `README.md` file looking good.

## Bonuse tasks

How to get bonuses? Every initiative will be counted, just don't forget to describe it in your `README.md`.

List of bonus tasks proposed:

1. Use different tools and platforms instead of what has been passed in the labs, for example, GitLab CI/CD, Netlify, etc. This will give you a bigger overview of technologies.
2. Use different languages (Java, Ruby, Python, etc.) to develop the application of part 1.
3. If you use the NodeJS application provided in the [courses/devops/modules/04.continuous-testing/assets/userapi](courses/devops/modules/04.continuous-testing/assets/userapi) folder, bring it with additional features:
  - more different API methods
  - more different unit/functional/integration tests
  - using another database (like MongoDB, MySQL, ...)
  - integrate a documenting package to your source code, for example, [Swagger UI](https://www.npmjs.com/package/express-swagger-generator)
4. Etc. 

## Grading system

| Subject                                                         |   Code    | Max. grade|
|:----------------------------------------------------------------|:---------:|:---------:|
| Enriched web application with automated tests                   |   APP     |    +1     |
| Continuous Integration and Continuous Delivery (and Deployment) |   CICD    |    +3     |
| Containerisation with Docker                                    |   D       |    +2     |
| Orchestration with Docker Compose                               |   DC      |    +3     |
| Orchestration with Kubernetes	                                  |   KUB     |    +4     |
| Infrastructure as code using Ansible                            |   IAC     |    +4     |
| Accurate project documentation in README.md file                |   DOC     |    +3     |
| Each bonus tasks                                                |   BNS     |    +1     |
| Each penalty                                                    |   PNL     |    -1     |

It is also taken into account:

- richness of the commit history
- accuracy and purity of the project (descriptions, source code, files structure)
- activity during course sessions
