---
copyright:
  years: 2017, 2019
lastupdated: "2019-09-08"

keywords: vpc, virtual private cloud, private cloud network, quick provisioning, logical isolation, security, cloud-native, workloads, BYOIP, high availability, ACL, Access control list, block storage volumes

subcollection: vpc

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:download: .download}
{:table: .aria-labeledby="caption"}
{:DomainName: data-hd-keyref="DomainName"}

# About Virtual Private Cloud
{: #about-vpc}

Use {{site.data.keyword.vpc_full}} to create your own space in {{site.data.keyword.cloud}}. A virtual private cloud (VPC) is a secure, isolated virtual network that combines the security of a private cloud with the availability and scalability of IBM's public cloud.
{:shortdesc}

## Logical isolation
VPC gives your applications logical isolation from other networks, while providing scalability and security. To make this logical isolation possible, the VPC is divided into subnets that use a range of private IP addresses. You can create subets in suggested prefix ranges, or bring your own public IPv4 address range to your IBM Cloud account. By default, all resources within the same VPC can communicate with each other over the private network, regardless of their subnet. 


You can create instances with up to 80 Gbps network bandwidth per instance. Each instance can be multi-homed, that is, you can create multiple network interfaces per instance.

## Storage capabilities
When you create an instance, a 100 GB block storage volume is automatically attached as a primary boot volume. To add secondary data volumes to your instance, create *block storage* volumes.

## Internet access
Two options are available for enabling your instances to communicate with the public internet:
* To enable all instances in a subnet to send outgoing traffic, attach a *public gateway* to the subnet.
* To enable communication to and from a particular instance, independent of whether the subnet is attached to a public gateway, associate the instance with a *floating IP*.

## Security
For instance-level protection, use *security groups* that act as virtual firewalls to restrict traffic for one or more instances.

## High availability
A *region* is the geographical location where you deploy the VPC's services, resources, and applications. Each region contains *zones*, which are logically-isolated data centers with independent infrastructures. You can deploy resources in multiple zones to achieve fault tolerance and high availability.  

## Next steps
To get started using the API and CLI, [set up your environment](/docs/vpc?topic=vpc-set-up-environment).
To learn how to create VPC resources, see these tutorials:

* [Using the {{site.data.keyword.cloud_notm}} console to create VPC resources](/docs/vpc?topic=vpc-creating-a-vpc-using-the-ibm-cloud-console)
* [Using the CLI to create VPC resources](/docs/vpc?topic=vpc-creating-a-vpc-using-cli)
* [Using the REST APIs to create VPC resources](/docs/vpc?topic=vpc-creating-a-vpc-using-the-rest-apis)

For a list of features not yet supported in VPC (early access), see [Limitations](/docs/vpc?topic=vpc-limitations).