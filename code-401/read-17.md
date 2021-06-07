# AWS: S3 and Lambda
## AWS Lambda
AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.

### What does serverless mean?
The concept of “serverless” computing refers to not needing to maintain your own servers to run these functions. AWS Lambda is a fully managed service that takes care of all the infrastructure for you. And so “serverless” doesn’t mean that there are no servers involved: it just means that the servers, the operating systems, the network layer and the rest of the infrastructure have already been taken care of, so that you can focus on writing application code.

## How does AWS Lambda work?
Each Lambda function runs in its own container. When a function is created, Lambda packages it into a new container and then executes that container on a multi-tenant cluster of machines managed by AWS. Before the functions start running, each function’s container is allocated its necessary RAM and CPU capacity. Once the functions finish running, the RAM allocated at the beginning is multiplied by the amount of time the function spent running. The customers then get charged based on the allocated memory and the amount of run time the function took to complete.

## Some of the most common use cases for AWS Lambda that fit these criteria are:

* **Scalable APIs**
* **Data processing**
* **Task automation**

## Benefits of using AWS Lambda
* **Pay per use**
* **Fully managed infrastructure**
* **Tight integration with other AWS products**

## Function limits
* **Execution time/run time**
* **Memory available to the function.**
* **Code package size**
* **Concurrency**
* **Payload size**

# Review, Research, and Discussion
* **Describe “The Cloud”**
"The cloud" refers to servers that are accessed over the Internet, and the software and databases that run on those servers. By using cloud computing, users and companies don't have to manage physical servers themselves or run software applications on their own machines.

* **What is a container (as it relates to computers and servers)?**
A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. ... Available for both Linux and Windows-based applications, containerized software will always run the same, regardless of the infrastructure.

* **What is auto-scaling?**
AWS Auto Scaling lets you build scaling plans that automate how groups of different resources respond to changes in demand. You can optimize availability, costs, or a balance of both. AWS Auto Scaling automatically creates all of the scaling policies and sets targets for you based on your preference.

* **What is bandwidth?**
Bandwidth is a measure of how much information a network can transfer. The volume of data that can be transported varies, impacting how effectively a transmission medium, such as an Internet connection, operates.

* **How do cloud providers compute service costs?**
When setting price, cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.

## **Term**
* **Server Instances** :A server instance is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

* **Container** in cloud computing is used to build blocks, which help in producing operational efficiency, version control, developer productivity and environmental consistency.

* **cloud services** refers to a wide range of services delivered on demand to companies and customers over the internet. These services are designed to provide easy, affordable access to applications and resources, without the need for internal infrastructure or hardware. From checking email to collaborating on documents, most employees use cloud services throughout the workday, whether they’re aware of it or not.

* **Cloud Architecture** refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources to solve business problems. Cloud architecture defines the components as well as the relationships between them.

* **AWS** stands for Amazon Web Services. ... AWS for beginners offers database storage options, computing power, content delivery, and networking among other functionalities to help organizations scale up. It allows you to select your desired solutions while you pay for exactly the services you consume only.
* **EC2/Beanstalk vs Heroku**:

Elastic Beanstalk is one layer of abstraction away from the EC2 layer. Elastic Beanstalk will setup an "environment" for you that can contain a number of EC2 instances, an optional database, as well as a few other AWS components such as a Elastic Load Balancer, Auto-Scaling Group, Security Group.  