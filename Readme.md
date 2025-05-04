# Create Virtual Machine
* In AWS ecosystem a vm is called EC2 instance
* ```AWS console``` --> we can create a vm using UI
* if we want to create 100 vm using the ui it is not a good practise
* So AWS provides us with apis for their services [ EC2 api ] so that automation is possible
* we normally write a script that makes use of these apis
* so if we want to create 10 vm each day and for 10 days we can run this script on each day
* the developers at amazon has exposed api for all its services
* we are now concerned about EC2 api
* when the request is send to the above api following the below conditions an EC2 instance is created
    * **valid** --> the format of the request must be correct
    * **authenticated**
    * **authorized** --> some users will not have permission to create an EC2 instance
* script makes an api call by following the above 3 conditions
---
* ```AWS CLI``` --> UI
* ```AWS Api using (Boto 3)```
    * using python along with this library called Boto3 we can directly make use the EC2 api or other service apis
* ```AWS CFT (Cloud Formation Template)```
    * we are using templates
* ```Terraform```
    * we can automate process in multiple cloud providers using Terraform
* ```AWS CDK```
    * specific to AWS
    * so it will have early access to any new services
    * if our organization is planning to stick with AWS for a longer time better to use CDK than terraform
---
* Refer Image 1
* Using all these methods we are talking to AWS api
* Remember EC2 instance or vm is an infrastructure
* What are the tools used for infrastructure automation ? 
    * AWS CLI,AWS CFT,Terraform
* Hybrid cloud model
    * different services in different cloud platform
    * Terraform is better for this as infrastructure must be maintained across different cloud platform
    
### Refrence

* [YouTube](https://www.youtube.com/watch?v=NJkMe9cdYEQ&list=PLdpzxOOAlwvIKMhk8WhzN1pYoJ1YU8Csa&index=5)