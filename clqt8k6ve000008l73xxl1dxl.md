---
title: "Unlocking Cloud Security: A Playful Guide to AWS IAM with a Toy Box Analogy"
seoTitle: "Mastering Cloud Security with AWS IAM"
seoDescription: "Unlock the secrets of robust cloud security with our in-depth guide to AWS IAM. Learn how to control access, manage users, and implement policies."
datePublished: Sun Dec 31 2023 08:34:44 GMT+0000 (Coordinated Universal Time)
cuid: clqt8k6ve000008l73xxl1dxl
slug: unlocking-cloud-security-a-playful-guide-to-aws-iam-with-a-toy-box-analogy
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1704010298785/704d8ac4-ade9-4512-84c2-43683c1956b0.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1704010826772/6abd1408-ea4e-42cf-a3d4-97b128ae71e4.png
tags: cloud-computing, devops, identity-and-access-management, devops-articles, aws-iam, devops-trends, devops-journey, cloud-security, devopscommunity, aws-amazonwebservices-cloudcomputing-scalability-5-innovation-businesstransformation-datasecurity-8-costeffective-techblog-awsservices-cloudtechnology-awsbenefits-digitaltransformation-awssecurity-awsforbusiness-cloudstorage-machinelearning-awsanalytics-awsnetworking-awscomputing, authentication-and-authorization-management, cloud-infrastructure-setup-company

---

In the rapidly changing world of cloud computing, AWS IAM plays a critical role in making sure that only the right people have secure access. IAM, which stands for Identity and Access Management, gives users the power to control who can do what, ensuring that only the necessary permissions are given out. It's more than just confirming who you are – IAM also provides a strong way to safely share and work together across different accounts. At its core, IAM policies are really important because they define what actions are allowed, making sure everything stays secure. In this blog, you will learn more about the significance of AWS IAM and how it contributes to maintaining robust cloud security.

Now, Let's Get Into the Story :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704006989904/fa9e950c-676f-479c-805f-c5273f9e3d6f.webp align="center")

# Real-Life Example:

imagine you have a big box of toys, and you want to share some of them with your friends, but you also want to make sure that only your closest friends can play with certain toys. This is where AWS IAM comes in, and it's like having a special helper to manage who can play with which toys.

So, let's say you have three friends: Timmy, Sarah, and Alex. Timmy is your best friend, so you want to let him play with all the toys. Sarah is a good friend, but not as close as Timmy, so you only want her to play with the cars and trucks. Alex is a new friend, and you're not sure yet, so you don't want him to play with any toys for now.

### Connecting the Story to IAM Service:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691912827054/6126d2c8-c15b-4a89-8773-28ec4e21ebbc.gif?auto=format,compress&gif-q=60&format=webm align="center")

In AWS IAM terms:

* Timmy is like the "Administrator" who can play with all the toys.
    
* Sarah is like a "User" who can only play with the cars and trucks.
    
* Alex is like a "Guest" who can't play with any toys yet.
    

# Understanding IAM's Building Blocks:

### 1) Users:

Imagine making a new person part of the security plan. It's like giving them a badge that lets them into a building. When someone joins a company, they get a special 'badge,' which is like a user profile. This profile lets them use cloud services in AWS. But it's not just about getting in – it's about saying what they're allowed to do once they're in. This is where policies come in.

### 2) Policies:

Policies are like rules that say what a person can do in the cloud. These rules decide what they can change, see, or use. Without policies, someone might get in but not be able to do much. Policies make sure people have the right permissions to do their jobs well. It's like giving someone keys to some rooms, but only letting them open certain doors.

### 3) Groups:

Imagine lots of people coming and going. Setting up access for every person can be a hassle, right? That's where groups come in. Think of groups as categories that help manage access. As a DevOps engineer, you can group people as 'developers,' 'QA engineers,' 'DB administrators,' and more. Instead of giving each person access one by one, you give access to groups. So, when a new person joins, you just put them in the right group – it's like giving them a membership card.

### 4) Roles:

Roles work a bit differently. Imagine an app needing access to a cloud service. It's not a person, but it still needs to get in. Roles act like temporary passes for this. For example, if an app needs data from a cloud database, you create a 'role' for it. This role lets the app in for a short time and specific tasks. It's like lending your friend your Netflix account for a movie night – you trust them, but you set limits.

By understanding these basic ideas, you'll be better at using AWS IAM and making your cloud setup more secure and smooth.

# Let's Do a Hands-on :

### Exercise :

As you probably know at this point, it's not recommended to work with the root account in AWS. For this reason, you are going to create a new account that you'll use regularly as the admin account.

1. Create a user with password credentials
    
2. Add the newly created user to a group called "admin" and attach to it the policy called "Administrator Access"
    
3. Make sure the user has a tag called the key `Role` and the value `DevOps`
    

### Solution :

1. Go to the AWS IAM service
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916595975/844fc50e-7997-46f3-a10f-8c4c1afc3d10.png?auto=compress,format&format=webp align="left")
    
2. Click on "Users" in the right side menu (right under "Access Management")
    
3. Click on the button "Add users"
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916619250/ce073607-63e6-42ae-a843-03b5f88b458e.png?auto=compress,format&format=webp align="left")

1. Insert the user name (e.g. Kelvin)
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916669632/92704dac-9fd7-4d54-9b89-fa92e8fb3036.png?auto=compress,format&format=webp align="left")

1. Select the credential type: "Password"
    
2. Set the console password to custom and click on "Next"
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916682800/63586b40-f25f-464f-b3fb-7e8d70e275e8.png?auto=compress,format&format=webp align="left")

1. Click on "Add user to group"
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916702510/d4e65cde-47c8-4507-8b1e-bb67b7a2af72.png?auto=compress,format&format=webp align="left")

1. Insert "admin" as the group name
    
2. Check the "Administrator Access" policy and click on "Create group"
    
3. Click on "Next: Tags"
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916717290/0413ba6b-3c1d-4e34-bcd7-8455193a3d9a.png?auto=compress,format&format=webp align="left")

1. Add a tag with the key `Role` and the value `DevOps`
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916785126/fcce85e2-47d2-4586-902d-b160cd3280ee.png?auto=compress,format&format=webp align="left")

1. then create on "Create user"
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1691916792639/f94108c8-756f-4cfb-aca2-7a2ee740cbc8.png?auto=compress,format&format=webp align="left")

# Conclusion :

To sum up, AWS Identity and Access Management (IAM) is like a guard for cloud setups. It uses users, policies, groups, and roles to make sure access is secure. Just like the bank controls who goes where, IAM gives out special keys, stopping chaos and problems. Policies shape access, groups manage users, and roles add security – all similar to controlled lending. Knowing these ideas helps you use AWS IAM better, making your cloud secure and efficient. The exercise shows how important IAM is by helping you create users and give them permissions, showing how to use IAM in real situations for better cloud security.

[**Twitter**](https://twitter.com/Kelvinparmar12) [**LinkedIn**](https://www.linkedin.com/in/kelvinparmar/) [**Hashnode**](https://kelvin-parmar.hashnode.dev/)