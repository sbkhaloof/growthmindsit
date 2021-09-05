# AWS: S3 and Lambda
## Review, Research, and Discussion
+ Describe “The Cloud”
### refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world.
+ What is a container (as it relates to computers and servers)?
### A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.
+ What is auto-scaling?
### AWS Auto Scaling monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it’s easy to setup application scaling for multiple resources across multiple services in minutes.
+ What is bandwidth?
### The maximum amount of data transmitted over an internet connection in a given amount of time.
+ How do cloud providers compute service costs?
### he three biggest cost centers related to a cloud environment include network, compute, and storage. Compute: Cost per GB of Virtual RAM Each organization has a unique set of requirements including use of CPU. Most providers calculate the cost of CPU by determining the respective company’s cost per GB of virtual RAM, which includes: Hardware operation: Providers look at the total amount of virtual RAM deployed in their public clouds and then divide that into the cost per rack unit of your hardware. Your costs may include licensing and usage-based subscription costs, depending on your virtual operating system. Hardware acquisition: This computation tells your provider how much it costs to acquire hardware for each GB of virtual RAM that you’ll be using. They also depreciate these costs over the hardware lifecycle. Your individual cloud computing infrastructure costs aren’t all that go into your price quote. Like IaaS cloud users, your quote includes a share of what it costs to power and cool the underlying infrastructure for the IaaS platform in the datacenter. Your price quote may also include charges related to software licenses, hosting, support and other service components. Sharing these costs with other organizations in the public cloud is what makes IaaS so cost-effective.
## Document the following Vocabulary Terms
+ Server Instances :
+ Containers: is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.
+ Cloud Services : are infrastructure, platforms, or software that are hosted by third-party providers and made available to users through the internet.
+ Cloud Architecture : defines the technology components that are combined to build a cloud, where resources are pooled through virtualization technology and shared across a network. 
+ AWS : Amazon web Services, it is a platform that provide a cloud computing services in general.
+ EC2/Beanstalk vs Heroku :
1. One of the first factors that most people consider when weighing their options between Heroku vs AWS Elastic Beanstalk is the pricing. While both Heroku pricing vs AWS pricing follow the pay-as-you-go method, the services vary according to the package that you select. As the application size increases, Heroku price could end up being twice as much as the cost incurred on AWS.
2. Supported Languages ; Both Heroku and Elastic Beanstalk have extensive support for multiple programming languages.
3. Performance With Scalability ; Heroku’s dyno-based scalability model works exceptionally well for startups and small-scale businesses. However, if the size of the app increases to a great extent, the system slows down and faces other issues as well. Therefore, Heroku servers are not recommended for large-scale apps. AWS Elastic Beanstalk, on the other hand, is highly recommended for businesses that operate on a larger scale.

## Preparation Materials
 ### ***AWS S3*** 
 #### Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance. This means customers of all sizes and industries can use it to store and protect any amount of data for a range of use cases, such as data lakes, websites, mobile applications, backup and restore, archive, enterprise applications, IoT devices, and big data analytics. Amazon S3 provides easy-to-use management features so you can organize your data and configure finely-tuned access controls to meet your specific business, organizational, and compliance requirements. Amazon S3 is designed for 99.999999999% (11 9's) of durability, and stores data for millions of applications for companies all around the world.
#### Benefits: 
1. Industry-leading performance, scalability, availability, and durability
2. Wide range of cost-effective storage classes
3. Unmatched security, compliance, and audit capabilities
4. Easily manage data and access controls
5. Query-in-place and process on-request
6. Most supported cloud storage service
### ***AWS Lambda Basics***
#### AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.
### ***CDN***
#### Content Delivery Network (CDN) : is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.




[Github view](https://github.com/sbkhaloof/growthmindsit)