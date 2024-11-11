# Compute - Amazon Elastic Compute Cloud (EC2)

One of the basic services provided on the cloud is compute service, which means that AWS provides you with the compute resources needed to run your applications. An example of a compute service is *Amazon EC2* (Elastic Compute Cloud), which represents a *virtual server* or *virtual machine* (the two terms are used interchangeably).

## What is a server? How is a virtual server different from a regular server?

A *server* is like a computer or a set of computers that hosts and runs your applications. It consists of physical hardware (CPU, RAM, storage, networking components), an operating system installed on top of the hardware, and finally the applications that run on top of the operating system.

When you run your application on the cloud, your application doesn't interact directly with the actual hardware. Instead, it interacts with virtual hardware, which is a software representation of the actual hardware that can emulate its behavior. So on top of the virtual hardware, an operating system can be installed to run your application. The virtual hardware, operating system and application are known as the components of a virtual machine or virtual server (a software representation or emulation of an actual server).

The benefit of this virtualization or abstraction is that you can create more than one virtual machine that shares the same underlying physical resources. This helps achieve efficient and cost-effective use of resources. The sharing of these resources is done through a software component called the *hypervisor*, which enables the sharing of the underlying hardware. The hypervisor distributes the underlying physical computing resources, such as CPU and memory, to individual virtual machines as required.

![Virtual servers vs physical servers](https://i.imgur.com/Y4cdQntGQ5iIWiLbfiV__w_7de59c9fc12042f395222b1eec4664f1_cukB8I-WMmbU-jyWDHr-gqCkoK-YxN3I2w__vLo0Z9YyfJ2CkO75czHNjRSCUdZoqCjERYDtwozU4paXZX8NdBLFuOkuJT_JIASPcz5MR622XUOb5BxQcuxlWIj6NpnPfL5JS2P5GmcVN0P0UpY9jl8)

## Amazon EC2

In AWS, these virtual machines or virtual servers are called Amazon Elastic Compute Cloud or Amazon EC2. EC2 is one of the primary building blocks that you may directly use to run your applications or indirectly use by interacting with other services built on top of EC2 instances.

"Elastic" in EC2 means that you can acquire the necessary compute and memory resources that you need for your work. When you run your applications on EC2 instances, you can configure as many instances as you need, and you only pay for what you use. When you no longer need an instance, you can stop or terminate it. You can also pick the size of an EC2 instance, where size corresponds to the amount of compute, memory, and network capabilities for a given instance. It's easy to resize based on your needs.

EC2 instances are grouped into several types, such as general purpose, compute optimized, memory optimized, storage optimized, and accelerated computing, which you can choose based on your use case.

AWS uses a specific naming convention for the instance types. For example, *t3a.micro *breaks down as follows:
* t: family name
* 3: generation
* a: optional capabilities
* micro: size

AWS offers a few different pay-as-you-go purchasing options for EC2 instances. By default, you can choose to set up and launch *on-demand* EC2 instances that give you compute capacity with no long-term commitments. If you want to save on cost, you can opt for EC2 *spot instances*, which are unused EC2 computing resources in the AWS cloud available at a discount compared to on-demand prices.

**References**
1. [Hardware virtualization](https://en.wikipedia.org/wiki/Hardware_virtualization)
2. [Virtual servers vs physical servers](https://www.vmware.com/topics/glossary/content/virtual-server.html)
3. [Physical servers vs. Virtual machines](https://www.geeksforgeeks.org/difference-between-physical-servers-and-virtual-machines/)
4. [What is hypervisor?](https://www.vmware.com/topics/glossary/content/hypervisor.html)
5. [What is virtualization?](https://www.vmware.com/topics/glossary/content/virtualization.html)
6. [Traditional virtualization primer](https://www.vmware.com/topics/glossary/content/virtual-machine.html)
7. [What is amazon EC2?](https://aws.amazon.com/ec2/)
8. [Amazon EC2 instance types](https://aws.amazon.com/ec2/instance-types/)
9. [Instance type naming conventions](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html#instance-type-names)
10. [EC2 instance purchasing options](https://aws.amazon.com/ec2/pricing/on-demand/)