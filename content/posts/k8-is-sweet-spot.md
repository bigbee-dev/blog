---
title: "Managed Kubernetes is the sweet spot between VM and Serverless"
date: 2021-08-09T15:08:27+06:30
---

When we are developing an app or SaaS product, we have to consider, where we deploy our services, how to release updates and make sure our services are available to customers. In this article, we will examine the pros and cons of all major cloud computing resources: Virtual Machine, Serverless, and Managed Kubernetes.

## Virtual Machine
The VM, Virtual Machine, could be the start of cloud computing. All major cloud providers provide VM as IaaS, Infrastructure as a  Service. VM is a server that you have total control over OS - which means you have to patch OS, install and configure applications yourself. Managing servers in a production environment is not an easy job, especially for a small startup company. It is also required more effort to automate deploying applications on VM. But, the best thing is - it is cheap.

**The Goods**: cheap.  
**The Cons**: you are on your own.

## Serverless
On the other hand, Serverless provides computing resources such as CPU, Memory, and Storage without managing underlying servers. Examples of Serverless are [here](https://aws.amazon.com/serverless/), [here](https://cloud.google.com/serverless) and [here](https://azure.microsoft.com/en-in/solutions/serverless/#overview).  With Serverless, we only need to focus on our applications. It is excellent for a small startup, but the downside is - most Serverless services are tied to cloud provider - _vendor locked-in_! Another important thing to consider is **cost** - it can get expensive easily when application scales.

**The Goods**: it just works.  
**The Cons**: expensive, vendor locked-in.

## Managed Kubernetes
In recent years, many major cloud providers, such as AWS, GCP, DigitalOcean, and Linode, offer **Managed Kubernetes** service. No more vendor locked-in. I want to emphasize that it is _managed service_ - which means I don’t need to set up and maintain the Kubernetes cluster. With the power of Kubernetes, we can streamline operations such as automate application deployments, monitoring, instance replication, cluster scheduling, and seamless application releases. And the cost is predictable - we need to pay a fixed amount for worker nodes. _Managed Kubernetes offer cheap, managed VM while also providing automation such as deploying, load balancing, and scaling_. The major challenge is the developer teams need knowledge to _use_ Kubernetes.

**The Goods**: cheap, managed services.  
**The Cons**: learning curve
