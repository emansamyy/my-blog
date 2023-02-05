---
layout: post
author: emansamyy
title: "Deploy High Availability Website on AWS"
date: '2022-6-14 21:45:35 +0200'
thumbnail: /assets/img/posts/Udacity_Project2.jpeg
category: ['DevOps','Deployment']
summary: This project is developed as part of the Udacity Advanced Cloud DevOps Nanodegree.
keywords: high availability website
permalink: /blog/high-availability-website/
---
## Infrastructure as Code (IaC)


    The launch configuration script is written inside the servers.yml
    file and it echoes that the app works but you can edit and add html
    files and related styling files to show that page instead of the message.
    Change the instance type according to requirements.
    The AMI changes according to regions, change it accordingly


### Security Groups and Roles


   - an IAM Role that allows instances to use the S3 Service.
   - The app communicates on the default HTTP Port: 80, so servers will need this inbound port open since you will use it with the Load Balancer and * the Load Balancer Health Check. As for outbound, the servers will need unrestricted internet access to be able to download and update their software.
   - The load balancer should allow all public traffic (0.0.0.0/0) on port 80 inbound, which is the default HTTP port. Outbound, it will only be using port 80 to reach the internal servers.
   - The application needs to be deployed into private subnets with a Load Balancer located in a public subnet. One of the output exports of the CloudFormation script should be the public URL of the LoadBalancer.





[click to view code](https://github.com/emansamyy/Deploy-a-High-Availability-Website)