# CIRCLE CI FOR CI/CD

## create an account on circleci.com

- create a new project
- select the github repo to use
- select the branch (main)
- in the .circleci folder, create a config.yml file
- add the environment variables to the project

## config.yml

- choose version 2.1
- on orbs

  - add the aws-elastic-beanstalk orb
  - add the aws-cli orb
  - add eb-cli orb

- on jobs

  - build step

    - checkout the code
    - install dependencies of frontend and backend in separate steps
    - build the frontend and backend in separate steps
    - save the build folder as an artifact

  - deploy step
    - checkout the code
    - install aws cli
    - configure aws cli with the access key and secret key
    - deploy the application to elastic beanstalk

- on workflows
  - add the build and deploy steps
  - require the build step to pass before the deploy step
  - require approval before the deploy step

## images found on the circleci-images folder
