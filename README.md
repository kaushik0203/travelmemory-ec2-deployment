# travelmemory-ec2-deployment
Deployment of Travel Memory application on AWS EC2 with load balancing Technologies Used MongoDB Atlas Express.js React.js Node.js AWS EC2 Application Load Balancer Nginx PM2 Deployment Steps 

Backend Setup Cloned GitHub repository Installed dependencies Configured environment variables Connected to MongoDB Atlas Started backend using PM2 

Frontend Configuration Updated backend URL in frontend Installed dependencies 

Reverse Proxy Configured Nginx to route traffic to backend 

Scaling Created two EC2 instances Deployed backend on both instances 

Load Balancer Created target group Registered EC2 instances Created Application Load Balancer 

 

Current Situation: Backend successfully set up on several EC2 instances The connection to MongoDB Atlas is working. Application can be accessed locally with curl Set up and created the Load Balancer Implemented scaling architecture 

But: 

Health checks on the load balancer still don't work. ALB DNS doesn't let me fully access the application 

Architecture Overview 

User → Application Load Balancer → EC2 Instance 1 
                 → EC2 Instance 2 

Both instances connected to MongoDB Atlas 

 

Screenshots (To be attached) 

EC2 instances running 

PM2 process status 

MongoDB connection 

Target group configuration 

Load balancer configuration 

curl output showing backend response 
