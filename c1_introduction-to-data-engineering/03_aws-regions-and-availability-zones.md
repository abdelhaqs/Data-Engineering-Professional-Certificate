# AWS Regions and Availability Zones

## AWS Regions
AWS hosts its data centers across many geographical areas known as regions. At the time of the creation of this course, AWS has 34 launched regions around the world. Each dot on this map represents a region, which contains a cluster of data centers spread across the geographical area.

*[AWS Global Infrastructure Map (This link shows the most up-to-date list of AWS regions)]*

Each AWS region is assigned a geographical name and a region code. The geographical name reflects the region's location. For example, in the United States, there is a region in Northern Virginia called the Northern Virginia Region (N. Virginia). This region has the code *us-east-1* meaning it was the first one created in the eastern US.

AWS regions are independent from one another, meaning your data is not replicated from one region to another without your authorization.

To host your applications or data pipelines, you need to choose an AWS region. Consider these four main factors:

* Latency: choose a region close to where your end users are located to minimize latency;
* Cost: the resource costs may differ between regions;
* Compliance: certain regulations may require hosting your data in a specific geographic region;
* Service availability: not all services are available in all regions.

## Availability Zones (AZs)
In each region, data centers are spread out into availability zones. Each region contains at least 3 isolated and physically separated availability zones. From Amazon's documentation about their global infrastructure: "AZs are physically separated by a meaningful distance, many kilometers, from any other AZ, although all are within 100 km (60 miles) of each other"(1).

Each availability zone contains a group of one or more discrete data centers with redundant power, networking, and physical security. All AZs in an AWS Region are interconnected with high-speed low-latency links.

AZs are assigned a code name. The code name consists of the region code followed by a letter. For example, *us-east-1a* represents an availability zone in us-east-1 (Northern Virginia Region).

The main purpose of having more than one availability zone within a region is to allow you to host your applications and data resources in multiple AZs for high availability and fault-tolerance. If one availability zone becomes unavailable due to power outage or natural disaster, your work will not be impacted.

**References**
1. [Regions and Availability zones](https://aws.amazon.com/about-aws/global-infrastructure/)
2. [AWS Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/)