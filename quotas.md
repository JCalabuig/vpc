---

copyright:
  years: 2018, 2019
lastupdated: "2019-08-28"

keywords: quotas, vpc, resources, limited, early access 

subcollection: vpc


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}

# Quotas
{: #quotas}

This document covers quotas for the {{site.data.keyword.vpc_full}} early access release and the resources available within it. To increase a quota for a particular resource, [contact support](/docs/get-support?topic=get-support-getting-customer-support).
{:shortdesc}


## VPCs
{: #vpc-quotas}

|   Resource     | Quota |
| ------- | :------: |
| Virtual private clouds | 5 per region|
| Subnets | 15 per VPC |
| Public Gateways | 1 per zone per VPC |
| Address prefixes | 15 per VPC |

## Virtual server instances
{: #vsi-quotas}

|   Resource     | Quota |
| ------- | :------: |
| vCPU |  20 per region  |
| RAM | 80 GB per region* |
| Network interfaces | 5 per instance |
| Floating IP addresses | 10 per zone |
| SSH keys | unlimited |

*based on host configuration ratio of 1:8 vCPU:RAM

## Security groups
{: #security-group-quotas}

|Resource|Quota|
|--------|-----|
|Security groups|5 per VPC|
|Rules|25 per security group|
|Remote rules|5 per security group|
|Network interfaces|5 per security group|

## Block storage volumes
{: #block-storage-quotas}

| Resource | Quota |
|----------|-------|
| Boot and secondary volumes | 750 total volumes per account |
| Secondary volumes per instance, attached when creating an instance |  4 secondary volumes |
| Secondary volumes per instance, for existing instances with fewer than 4 cores | 4 secondary volumes |
| Secondary volumes per instance, for existing instances with 4 cores or more | up to 12 secondary volumes |

**Note** The volume attachment limits are recommended but not strictly enforced in the early access release. Depending on your OS environment, you might be able to attach more secondary volumes to an instance.
