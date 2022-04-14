
# Exam instructions

You will receive 20 **multiple and single choice questions** (MCQ, in French). To prepare, you must review all of the course modules and continue working on your project for practice.

There will be 2 types of questions:

- Familiarity with the core CLI commands of the tools and understanding of configurations
- Understanding the passed concepts

Good luck!

## Example questions

### Question 1

You have the following `docker-compose.yml` file:

```yaml
version: "3.8"
services:
  web:
    build: .
    ports:
      - "3000:5000"
  redis:
    image: redis
    volumes:
      - /usr/data:/data
```

Choose correct option(s) where "web" service is accessible and "redis" service attaches data:

* [ ] A: On host: URL - `localhost:3000`, folder - `/usr/data`
* [ ] B: On host: URL - `localhost:5000`, folder - `/data`
* [ ] C: In container: URL - `localhost:3000`, folder - `/data`
* [ ] D: In container: URL - `localhost:5000`, folder - `/usr/data`

### Question 2

Which command(s) stop(s) and not remove(s) a running container (where `$CONTAINER` is a container name or a container ID)?

* [ ] A: `docker kill $CONTAINER`
* [ ] B: `docker rmi $CONTAINER`
* [ ] C: `docker stop $CONTAINER`
* [ ] D: `docker rm $CONTAINER`

### Question 3

The Manifesto for Agile Software Development includes the following item(s):

* [ ] A: Processes and tools over individuals and interactions
* [ ] B: Working software over comprehensive documentation
* [ ] C: Customer collaboration over contract negotiation
* [ ] D: Following a plan over responding to change

### Question 4

What Ansible does not provide?

* [ ] A: Cloud provisioning
* [ ] B: Configuration management
* [ ] C: Container orchestration
* [ ] D: Application deployment
