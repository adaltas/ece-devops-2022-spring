
# ECE DevOps course

Materials for the DevOps course at ECE.

## Modules

1. Introduction to DevOps
2. Source Control Management (SCM)
3. Continuous Testing | Building application on Node.js
4. Continuous Integration & Continuous Delivery (CI/CD) | with GitHub Actions and Heroku
5. Infrastructure as code (IaC) | with Ansible
6. Containerization | with Docker
7. Containers orchestration | with Kubernetes
8. Cloud-native applications. Microservice architecture | with Istio
9. Monitoring | with Prometheus and Grafana

## Assignment

The course assignment is consist of:

1. Participation
2. Project
3. MCQ exam

## Usage

### Reading slides' content

Navigate inside the [`./courses/devops`](courses/devops) folder to read the raw material and access the labs. The module's folders contain following files:

- `index.md` - materials for the module
- `lab.md` - labs description
- `homework.md` - homework description
- `lab` folder - assets provided for the labs
- `image` folder - images used in the `.md` files

### Access online slides

The slides are available on Netlify as a static website - [ece-devops-2022-spring.netlify.app](https://ece-devops-2022-spring.netlify.app/).

[![Netlify Status](https://api.netlify.com/api/v1/badges/5ad68890-b1bf-4ca4-aebc-83ff9a773728/deploy-status)](https://app.netlify.com/sites/ece-devops-2022-spring/deploys)

### Build slides locally as a static website

Run the following commands to get the site up and running.

```
# Clone the repository
git clone https://github.com/adaltas/ece-devops-2022-spring.git devops
cd devops/gatsby
# Download the dependencies
npm install
# Start the development server
npm run develop
# If you have problem, try
npm run clean && npm run develop
```

## Author

Sergei Kudinov   
sergei@adaltas.com     
Developer and Big Data Engineer at [Adaltas](https://www.adaltas.com/)
