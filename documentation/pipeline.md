*This is the breakdown of the circle ci config file*

## Commands

### install_client
The purpose of this command is to install the client dependencies if they weren't cashed. If they were cashed, they won't be installed & will be loaded from the cashe to save time.

### install_server
This is the same as [install_client] but for the server "API".

## Jobs

### build
Here, circleci installs **NPM dependencies**, **checkout**, **install** then **build** both the client & server.

### test
Here, it installs **NPM dependencies**, **checkout**, **install** then run the **test** script for both the client & server.

### deploy
And here, it installs **NPM dependencies**, setup the **AWS CLI** & **Elastic Beanstalk**, **checkout**, **install** then deploy both the client & server.

## Workflow

### build
- First, circleci execute `build` which gets triggered once any change happen on the specified branch.
- Then execute `test` which requires `build`
- Then execute `deploy` which requires `test`
