# amplify-react-graphql

## Purpose
The purpose of this project was to learn how to deploy a full stack notes app on AWS.
## Intention
AWS is an important tool that many companies use, and knowing how to use it is a valuable skill for any developer to have. 

My goal wasn't to develop an overly complicated web app, which is why I stuck to a basic CRUD notes app. I did implement an image storage / retrieval feature as well. 

## Problems and Solutions

### Hosting

**Problem:** Hosting on AWS required understanding their tools and knowing which one to go with

**Solution:** I went with AWS Amplify. It provides a Git-based CI/CD workflow for building, deploying, and hosting single-page web applications or static sites with serverless backends. It also supports continuous deployment which was helpful

**Takeaway:** I know know how to deploy a web app to AWS Amplify

### Authentication

**Problem:** A basic CRUD note taking app needs a way to save a specific users' notes. I needed to add a sign in, up feature which requires authentication

**Solution:** Sticking with AWS, I authenticated a user using the Amplify CLI, and leaveraged Amazon Cognito, which managed user identities. The Amplify UI component library helped creating an entire user authentication workflow, from signing up, verifying emails, reseting passwrods, and signing in

**Takeaway:** I know how to authenticate users with just a few lines of code now

### Databse and Storage

**Problem:** A user's notes needed to be saved somewhere, so I needed to use an API which is backed by some database.

**Solution:** Again, sticked with AWS, I used a GraphQL API that uses AWS AppSync which is backed by Amazon DynamoDB. Finally, I added storage for pictures using Amazon S3

**Takeaway:** I can now build a fully functioning CRUD app, hosted entirely on AWS, with authentication and storage features

## Additional

A deployed version of the application can be found [here](https://main.d2sfonb0rgw1sr.amplifyapp.com/)