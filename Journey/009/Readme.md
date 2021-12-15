![placeholder image](https://dailymedia.case.edu/wp-content/uploads/2017/11/28152832/computer-code.jpg)

# Finishing the second project

## Introduction

This project was easier than the first one, mainly because I was more used to the way things work with Terraform and AWS. The project [COM03-AWS200 - Create an Auto Scaling Group](https://github.com/100DaysOfCloud/100DaysOfCloudIdeas/blob/master/Projects/COM/COM03/COM03-AWS200.md) is from 100DaysOfCloudIdeas too, but it is shorter than the first one.

## Prerequisite

I used the code of the first project as a basis for this project.
## Use Case

Objectives
You need to complete the following:

    Create a Launch Configuration
    Create an Auto Scaling Group with a minimum of two and a maximum of five EC2 instances
    Terminate one instance manually
    After the ASG is in place, increase the desired number of instances to three
    Delete all the resources you created

You need to answer the following:

    What are the key differences between a Launch Template and Launch Configuration?
    - Launch Configuration can't be modified, to make changes it has to be replaced. Launch Templates can be changed and you can choose the specific version of the launch template that the group uses to launch EC2 instances.
    What happens if you terminate one of the running instances in an ASG manually?
    - Another instance will be launched to replace the terminated instance.
    How can you set and change the minimum, desired, and maximum number of instances in an ASG?
    - In the Autoscale group configuration. In my case, I used terraform code to do it.
    Based on what metrics can an ASG spin up / spin down instances?
    - Based on a schedule, based on demand, or preditive scaling.
    What EC2 configuration settings can you set in a Launch Template/Configuration?
    - AMI, security groups, 
    Can you use Spot instances with a Launch Template/Configuration?
    - Yes, it can be done.
    How many subnets and regions can a single ASG utilize?
    - Just one.
    What is the difference between "desired capacity" and "minimum capacity"?
    In which order will EC2 instances be terminated in case of a scale-in event?

## ☁️ Cloud Outcome

Along with writing the code of this project, I could access the AWS console and check the progress of instance creation and, I could terminate instances and see them being recreated by the Autoscale Group.

### The final result

The code is available at my repository for this project (https://github.com/eduardoegito/COM03-AWS200)
## Social Proof

The posts that show that I shared my process on Twitter or LinkedIn are available below.

[Tweet post](https://twitter.com/eduardoegito/status/1471239554489372679)

[LinkedIn post](https://www.linkedin.com/posts/eduardoegito_github-eduardoegitocom03-aws200-activity-6877005441553973248-f6ow)