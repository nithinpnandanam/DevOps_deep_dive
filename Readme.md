# Connect to an instance and AWS CLI
---
* We can connect to an EC2 instance using the UI.
* a terminal will be available to us in the website
---
* We can also connect an EC2 instance through our own terminal 
* when cretaing an instance we would have downloaded a pem file that has a ```key-pair``` 
* step 1 --> ```chmod 600 /home/nithin/AWS/test-1.pem```
    * for updating the permission
* step 2 --> ```ssh -i /home/nithin/AWS/test-1.pem ubuntu@3.107.67.87```
    * 3.107.67.87 is the public ip
* This method gives you shell access to the EC2 instance
* We are directly connecting from your local terminal to the EC2 instance over SSH.
---
* if we do not want to use the instance we can 
    * stope the instance
    * then terminate the instance

## Below is a method to interact with AWS itself (manage EC2, S3, Lambda, etc.), not individual machines.
---
* Using AWS CLI
    * go to security credentials >> create access key >> store the access key and password
    * ```aws configure ```
    * you set up credentials (AWS Access Key ID, Secret Access Key) in your local machine to interact with AWS services via the AWS CLI.
    ```aws ec2 describe-instances```
    ```aws s3 ls```
    * These commands talk to AWS APIs and control or query AWS resources from your local machine, but they do NOT log you into the instance like SSH
    * Use AWS CLI when you want to list EC2 instances, start/stop them, create new ones, or interact with other AWS services without logging in
---
### Refenece
* [YouTube](https://www.youtube.com/watch?v=cN4pt5KQ9eA&list=PLdpzxOOAlwvIKMhk8WhzN1pYoJ1YU8Csa&index=7)