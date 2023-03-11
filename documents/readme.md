### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Infrastructure

```
- User send input into fronend in S3

- Frontend take that request to backend in EB environment to retrive data from database in RDS

- Data is sent to backend that send response to frontend to show it to the user.


```

### Pipeline

```
- Pipeline setup environments node, rb and aws-cli in orbs.

- The jobs which are commands that first build the application, then deploy it when it ensures that it works successfully.

- The workflow that arrange the steps and make a holder for approval deployment

```

