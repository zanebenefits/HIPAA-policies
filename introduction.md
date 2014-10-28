# Introduction

Zane Benefits is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Customers. As providers of compliant, hosted software as a service, Zane Benefits strives to maintain compliance, proactively address information security, mitigate risk for its Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by Zane Benefits to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for Zane Benefits Customers.

Zane Benefits provides secure and compliant cloud-based software solutions. These hosted software products include ZaneHealth, ZaneHRA, GroupHRA and ZanePRA. These products are cited throughout polices as Software as a Service or SaaS since Customers in each of these products inherit the same policies, procedures, and obligations from Zane Benefits.

## Software as a Service (SaaS)

SaaS Customers utilized hosted software from Zane Benefits. These customers are deployed into compliant containers run on systems secured and managed by Zane Benefits. Zane Benefits makes every effort to reduce the risk of unauthorized disclosure, access, and/or breach of SaaS Customer data through network (firewalls, dedicated IP spaces, etc) and server settings (encryption at rest and in transit, etc).

## Compliance Inheritance

Zane Benefits provides compliant hosted software for its Customers. Zane Benefits signs business associate agreements (BAAs) with its Customers. These BAAs outline Zane Benefits obligations and Customer obligations, as well as liability in the case of a breach. In providing infrastructure and managing security configurations that are a part of the technology requirements that exist in HIPAA and HITRUST, as well as future compliance frameworks, Zane Benefits manages various aspects of compliance for Customers. The aspects of compliance that Zane Benefits manages for Customers are inherited by Customers, and Zane Benefits assumes the risk associated with those aspects of compliance. In doing so, Zane Benefits helps Customers achieve and maintain compliance, as well as mitigates Customers risk.

Certain aspects of compliance cannot be inherited. Because of this, Zane Benefits Customers, in order to achieve full compliance or HITRUST Certification, must implement certain organizational policies. These policies and aspects of compliance fall outside of the services and obligations of Zane Benefits.

Below are mappings of HIPAA Rules to Zane Benefits controls and a mapping of what Rules are inherited by SaaS Customers.

## Zane Benefits Organizational Concepts

The physical infrastructure environment is hosted at [Amazon Web Services (AWS)](http://aws.amazon.com/compliance/). The network components and supporting network infrastructure is contained within AWS infrastructure and managed by AWS. Zane Benefits does not have physical access into the network components. The Zane Benefits environment consists of Apache web servers, Linux PHP application servers, and MySQL database servers using EC2 security groups.

Within the Zane Benefits Platform on AWS, all data transmission is encrypted and all hard drives are encrypted so data at rest is also encrypted; this applies to all servers - those hosting PHP, databases, etc. Zane Benefits assumes all data *may* contain ePHI, even though our Risk Assessment does not indicate this is the case, and provides appropriate protections based on that assumption.

There is data and network segmentation in place with AWS. Hosted load balancers segment data across a dedicated Virtual Private Cloud. Additionally, Zane Benefits has implemented strict logical access controls so that only authorized personnel are given access to the internal management servers. The environment is configured so that data is transmitted from the load balancers to the application servers over an SSL encrypted session.

The Apache web servers and PHP application servers are externally facing and accessible via the Internet. The database servers, where the ePHI resides, are located on the internal Zane Benefits network and can only be accessed from whitelisted IP addresses and with the proper credentials. The access to the internal database is restricted to a limited number of personnel and strictly controlled to only those personnel with a business justified reason.

## Version Control

Policies were last updated October 28th, 2014.