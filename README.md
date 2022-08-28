# udagram

It's a [website](http://ahmed-bucket-1.s3-website-us-east-1.amazonaws.com) where you can register, login & create new posts.

## Usage "Locally"

### Database

- Create a database called "udagram"

### Navigate to udagram-frontend, then:

- To build the frontend: `npm run build`
- To start the frontend: `npm run start`
- To test the frontend: `npm run test`
- To deploy the frontend: `npm run deploy`

### Navigate to udagram-api, then:

- To build the frontend: `npm run build`
- To start the frontend: `npm run dev`
- To test the frontend: `npm run test`
- To deploy the frontend: `npm run deploy`

## More Info

- You can find the required screenshots under "documentation/screenshots" folder in the root directory.
- The circleci configuration file, elastic beanstalk & documentation files can be found in the GIT repository

### Message to the reviewer

When I try to login, I get `HTTP failue response for the API URL: 0 Unknown Error` eventhough it is working fine on my local device, I can see the APIs working via Postman & access the database using pgAdmin. I checked a lot but couldn't figure it out.
Can you please guide me to fix it?