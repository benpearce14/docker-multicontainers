# Docker Multicontainers in Action

This application demonstrates how multiple services in multiple Docker containers can be stitched together and hosted on an AWS account.

This particular setup contains the following services:

1. Nginx Router
2. Redis Database
3. Postgres Database
4. Express API
5. React Frontend
6. Node.js worker

This application is intentionally overcomplicated - this is clearly not how this particular app would be designed, and is instead a demonstration of the use of multiple Docker containers. This project also contains a github action to push each of the containers to your dockerhub account, and to push your images to AWS Elastic Beanstalk (EB).

You will need to confingure some action secret on your fork of the repository:

- `DOCKER_USERNAME` - your username for Docker
- `DOCKER_PASSWORD` - your password for Docker
- `AWS_ACCESS_KEY` - your AWS access key
- `AWS_SECRET_KEY` - your ASW secret key
- `AWS_APP_NAME` - your application name on EB
- `AWS_ENV_NAME` - your environment name on EB
- `AWS_BUCKET_NAME` - your AWS S3 bucket name
- `AWS_REGION` - your AWS region
