---
title: "Connecting to Amazon EC2 Instances Using SSH"
seoTitle: "Connecting to Amazon EC2 Instances Using SSH"
seoDescription: "Connecting to Amazon EC2 Instances Using SSH"
datePublished: Sun Jan 21 2024 07:27:31 GMT+0000 (Coordinated Universal Time)
cuid: clrn6emio00010alf2xmc3zin
slug: connecting-to-amazon-ec2-instances-using-ssh
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1705822003810/bb940a1e-76f0-45fb-8638-57762459a9aa.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1705822038673/19c8058f-c268-4b35-bd81-127c573bbeac.png
tags: aws, aws-certified-solutions-architect-associate, aws-ec2, amazon-ec2-ssh-connection, connect-to-ec2-instance-without-third-party-software, ssh-key-pair-for-ec2, securely-connect-to-aws-ec2-using-ssh, amazon-linux-ubuntu-ec2-ssh-tutorial, windows-ssh-client-for-amazon-ec2, step-by-step-ec2-ssh-guide, ssh-connection-to-aws-cloud-server

---

## Introduction

Amazon Web Services (AWS) has become a cornerstone in the world of cloud computing, providing scalable and reliable infrastructure for businesses and individuals alike. Amazon EC2 (Elastic Compute Cloud) is a popular cloud computing service that allows users to run virtual servers in the cloud. One of the common ways to connect to an EC2 instance securely is through SSH (Secure Shell). In this guide, we'll walk you through the steps to connect to an EC2 instance using the built-in SSH client, without the need for any third-party software.

## Step 1: Launching an EC2 Instance

Before you can connect to an EC2 instance, you need to launch one. This involves selecting the appropriate Amazon Machine Image (AMI), configuring instance details, adding storage, and setting up security groups. We already created in our last blog you can also that blog here: [https://kelvin-parmar.hashnode.dev/aws-ec2-empowering-your-cloud-journey-with-virtual-servers](https://kelvin-parmar.hashnode.dev/aws-ec2-empowering-your-cloud-journey-with-virtual-servers)

After creating a EC2 instance click on Connect button where you can find all the details to connect in you local machine using SSH.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705818036208/53b65b92-7f79-456c-b076-9a09fa180c7b.png align="center")

## Step 2: Generating SSH Key Pair

Security is paramount when it comes to managing AWS resources. To secure the communication between your local machine and the EC2 instance, SSH key pairs are used. The guide emphasizes the importance of creating and managing SSH key pairs for a secure connection. It walks you through the process of generating an SSH key pair using the ssh-keygen command.

## Step 3: **Get Your Key Pair**

When launching an EC2 instance, you specify a key pair. Ensure you have the private key file (.pem) associated with that key pair.

Open yout terminal where your .pem file is stored. Here in my case I downloaded into downloads folder so opened into my cmd.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705817564212/7b90e8ae-4905-4816-aebf-7125a5d4ecce.jpeg align="center")

After that run the below command. Replace `"test-ec2.pem"` with the actual path to your private key file.

```bash
chmod 400 "test-ec2.pem"
```

## Step 4: Connect Using SSH

Use the `ssh` command to connect to your EC2 instance. Adjust the following command with your information:

```bash
ssh -i /path/to/your/keyfile.pem ec2-user@your-instance-ip
```

Replace `/path/to/your/keyfile.pem` with your private key file path and `your-instance-ip` with the EC2 instance's public IP address or DNS name. Note that the default username for Amazon Linux instances is usually `ec2-user`.

For example:

```bash
ssh -i "test-ec2.pem" ubuntu@ec2-13-126-13-170.ap-south-1.compute.amazonaws.com
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705817982766/f31a5d67-3552-4c2e-87c3-9189097c4291.jpeg align="center")

## Bonus Tip: Windows Users

If you're using Windows, you can utilize the built-in SSH client or a tool like PuTTY. However, this guide demonstrates that, even on Windows, you can opt for the command line without the need for additional software.

## Conclusion

By following these simple steps, you can connect to your Amazon EC2 instance securely using SSH. Whether you're using a Mac, Linux, or even Windows with its built-in SSH client, this guide eliminates the need for third-party software, providing a streamlined and secure connection experience.

If you find it helpful then like it and subscribe to more articles on aws cloud journey.

[**Twitter**](https://twitter.com/Kelvinparmar12) [**LinkedIn**](https://www.linkedin.com/in/kelvinparmar/) [**Hashnode**](https://kelvin-parmar.hashnode.dev/)