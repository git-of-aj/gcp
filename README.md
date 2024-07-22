# Day1 - [GCP WAF](https://cloud.google.com/architecture/framework/system-design)
- start here : https://cloud.google.com/docs/overview
- IAM starts : https://cloud.google.com/docs/authentication
--------
*WAF*
- region : https://cloud.google.com/architecture/framework/system-design/geographic-zones-regions
- projects,hierachy: https://cloud.google.com/architecture/framework/system-design/resource-management
- network design: https://cloud.google.com/architecture/framework/system-design/networking

# ACE vs PCA 
Focused on tasks that Cloud Engineers perform in day to day job!

### Professional Cloud Architect

Understand business and technical requirements

Design cloud solutions that meet your functional and non-functional needs

**GCP Services are the same**:

BUT your perspective should be different

With Professional Cloud Architect

You need to know the services

AND learn to build highly resilient, highly available, scalable, secure, performant solutions that have

low cost!

Sounds Complex??

(Don't worry) We will understand each of these as we go further

# Scalability 
system is handling 1000 transactions per second. Load is expected to

increase 10 times in the next month

> Can we handle a growth in users, traffic, or data size without any drop in performance?

Does ability to serve more growth increase proportionally with resources?

Ability to adapt to changes in demand (users, data)

What are the options that can be considered?

Deploy to a bigger instance with bigger CPU and more memory

Increase the number of application instances and setup a load balancer

