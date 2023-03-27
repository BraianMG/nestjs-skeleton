<p align="center">
  <a href="http://nestjs.com/" target="blank">
    <img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" />
  </a>
</p>

<h1 style="text-align: center; margin-bottom: -10px; font-size: 30px;"><strong>NestJs-skeleton</strong></h1>

---

<div id="top"></div>

<details>
  <summary style="font-size: 25px"><strong>Table of Contents</strong></summary>
  <ol>
    <li>
      <a href="#about-the-project">About the project</a>
      <ul>
        <li><a href="#description">Description</a></li>
        <li><a href="#used-technologies">Used technologies</a></li>
        <li><a href="#features-offered-by-this-skeleton">Features offered by this skeleton</a></li>
      </ul>
    </li>
    <li>
      <a href="#setup">Setup</a>
      <ul>
        <li><a href="#for-development">For development</a></li>
        <li><a href="#for-production">For production</a></li>
      </ul>
    </li>
    <li><a href="#stay-in-touch">Stay in touch</a></li>
  </ol>
</details>

---

## __About the project__

### __Description__

This repository is a skeleton with the bases to start a new API (REST and GraphQL) with the NestJs framework.

<p align="right">(<a href="#top">Back to top</a>)</p>

### __Used technologies__

- [NodeJs v16.19.0](https://nodejs.org/es/)
- [NestJs](https://nestjs.com/)
- [TypeORM](https://typeorm.io/)
- [Jest](https://jestjs.io/)
- [PostgreSQL](https://www.postgresql.org/)
- [GraphQL](https://graphql.org/)
- [Apollo GraphQL](https://www.apollographql.com/)
- [Docker](https://www.docker.com/)

<p align="right">(<a href="#top">Back to top</a>)</p>

### __Features offered by this skeleton__

<!-- - Base CRUD -->
- ESLint and Prettier configured
- Basic file structure defined
- Environment configured to perform unit tests with Jest and Supertest
<!-- - Módules:
  - Auth
  - User
  - Profile -->

<p align="right">(<a href="#top">Back to top</a>)</p>

## __Setup__

### __For development__
- Create .env file from .env.example and populate with corresponding values
- Indicate the __container name__ for the app in the __docker-compose.yml__ file replacing "__myDB__" with the corresponding name
- Have Docker installed and running
- Install dependencies: `yarn install`
- Raise database image: `docker-compose up -d`
- Run the app: 
  - Development: `yarn run start`
  - Watch mode: `yarn run start:dev`
  - Production mode: `yarn run start:prod`
- Run tests: 
  - Unit tests: `yarn run test`
  - e2e tests: `yarn run test:e2e`
  - Test coverage: `yarn run test:cov`

<p align="right">(<a href="#top">Back to top</a>)</p>

### __For production__
- Create .env.prod file from .env.example and populate with corresponding values (optional)
- Indicate the __container name__ for the app in the __docker-compose.prod.yml__ file replacing "__myDB__" with the corresponding name
- Indicate the __image__ name for the app in the __docker-compose.prod.yml__ file replacing "__imagaNameForMyApp__" with the corresponding name
- Have Docker installed and running
- Build app: `docker-compose -f docker-compose.prod.yml --env-file .env.prod up --build`
  - Note: By default, docker-compose uses the .env file, so if you have the .env file and configure it with your production environment variables, it would suffice: `docker-compose -f docker-compose.prod.yml up --build`
- Run app: `docker-compose -f docker-compose.prod.yml --env-file .env.prod up`
- Rename: `docker tag <app name> <docker hub user>/<repository name>`
- Login to Docker Hub: `docker login`
- Upload image: `docker push <docker hub user>/<repository name>`

<p align="right">(<a href="#top">Back to top</a>)</p>

### __Stay in touch__

- Author - [Braian Gonzales](https://kamilmysliwiec.com)
- Website - [https://braiangonzales.netlify.app/](https://braiangonzales.netlify.app/)
- Email - [braian.gonzales77@gmail.com](mailto:braian.gonzales77@gmail.com)
- LinkdIn - [in/braiangonzales/](https://www.linkedin.com/in/braiangonzales/)

<p align="right">(<a href="#top">Back to top</a>)</p>
