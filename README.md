# opencuts-client

Project Goals:
* Continue my learning of React.js 
* Take on a new challenge: Use AWS/Python to build my backend
* Create a web app for Barbers can use to manage appointments

Itinerary:
[x]Setup Backend using AWS services: DynamoDB, S3 Buckets, Cognito(user auth), Lambda(Python), and API Gateway
[x]Build a React App
[x]Deploy site using serverless AWS

Progress Notes:

Backend:

* Simply setting up your AWS account/applications can be time consuming. There are many options. Some options CANNOT be changed  once the initials settings are in place. An example of this is when setting the user authentication settings, if you choose to ask your user to use a username to login, once that is set, you cannot change it to allow them to use simply their email. It will be looking for a username. This was a bit of a setback for me, so I figured I’d throw it out there.
* Setting up a DynamoDB table was rather easy. DynamoDB is a managed, NoSQL database. DynamoDB makes it extremely easy to update your tables. It’s flexible, and I think I will enjoy using it as I continue to scale up this project.
* Setting up the S3 bucket was also a breeze. BUT, make sure you copy ALL the information the give you down somewhere. You are constantly required to provide 'clientIds' and ‘keys’ throughout the process of building a backend on AWS.
* Make sure to update the CORS permission tag correctly. Google has some good info on what settings to use.
* Amazon Cognito is really cool when it come to setting up user auth for your site. BUT, I think this is where this project has become a bit of a struggle. Cognito has all kinds of COOL options as far as how you can allow your users to access your site. You can login in popular ways like using your Google account, or Facebook even! Sounds great right?!? It is great. I’ll admit it. But, there are so many rabbit-holes there, and they got me. At this point in my project, I’m having token issues. I can seem to POST data. It’s been a bit of a nightmare to try and work out these issues simply using online documentation provided by Amazon or StackOverflow, but I feel like I can get it resolved with a little more trial and error.
* Next step was making this project ‘serverless’. API Gateway was an easy way to setup the API, and seems like it would be easy to maintain going forward, which I thought was nice. API Gateway works with AWS Lambda. Lambda ended up confusing me, because it’s Python-based. Lambda is a lot like an arrow function is to javascript. Different syntax. Now that I’ve taken on learning new programming languages, I do like to clean up my code as much as possible, so I do like to try to learn ways to DRY out my code. Just my opinion, I like to learn shortcuts.
* The serverless framework made it easy to get up and running, and to create a project. (https://serverless.com/)
* After building the API, deploying the backend wasn’t too hard. AWS instructions are pretty clear. 

Frontend:

* React.js… after 900 youtube videos, classwork, reading different strategies online. I might know how to use it properly. Might.
* Learned how to integrate bootstrap with React. Something I’ve found to be very, very useful.
* React Router. I think I may have issues here. Can’t really have a single-page app with authentication without it, so I’m still learning it. I feel like I’m getting better with managing state.
* AWS Amplify integrates the backend with the React.js frontend. (It also works with iOS & Android… Future Goals.)
* I’ve gotten as far as creating different components that interact very well together on the frontend, but there are issues connect to the backend. Signup/Login works, but I believe there is an authentication issue when trying to create new appointments. This is where I’m current at in this project. I’m working on straightening out the authentication errors.
