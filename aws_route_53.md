
AWS Route 53 - 

1. Highly available and scalable cloud DNS webservice.
    1. DNS translates names like (www.google.com) to ip addresss like (192.3.x.x)
    2. Can configure DNS health to route traffic to healthy endpoints or to monitor health of application.
    3. DNS request are called `queries`.
2. Fully compliant IPv6.
3. Applicaiton can leverage for internal(aws cloud) and external(outside world) DNS resolution.
4. Manage traffic globally with variety of routing types, to ensure low lattency, fault tolerant architecture.
    1.  Latency Based Routing.
    2.  Geo DNS.
    3.  Geoproximity.
    4.  Weighted Round Robin.
5. Traffic Flow’s simple visual editor helps to visualize the real-time routing of user-data to application endpoints.
6.  Services
    1.  Domain name registration.
    2.  Health check webservices.
    3.  User can create and manage public DNS records.
    

## Getting Started

1.  You can configure with AWS Management Console or Route 53's API, DNS records are organized into “hosted zones”


### Security
1.  You can control management access to your Amazon Route 53 hosted zone by using the AWS Identity and Access Management (IAM) service.

### Price

#### Price > Hosted Zone
1. Hosted zones are billed once when they are created and then on the first day of each month.
2. Hosted zones have a grace period of 12 hours--if you delete a hosted zone within 12 hours after you create it, we don't charge you for the hosted zone.
3. After the grace period ends, we immediately charge the standard monthly fee for a hosted zone.

### Logging
1. You can configure Amazon Route 53 to log information about the queries that Route 53 receives
2. When you configure query logging, Amazon Route 53 starts to send logs to CloudWatch Logs.
3. You use CloudWatch Logs tools to access the query logs.

### Difference

#### Domain vs Hosted Zone

Domain  | Hosted Zone
------------- | -------------
 A domain is a general DNS concept like (github.com etc).  |  A hosted zone is an Amazon Route 53 concept.

A hosted zone is analogous to a traditional DNS zone file; it represents a collection of records that can be managed together, belonging to a single parent domain name. All resource record sets within a hosted zone must have the hosted zone’s domain name as a suffix.

For example, the amazon.com hosted zone may contain records named www.amazon.com, and www.aws.amazon.com, but not a record named www.amazon.ca. You can use the Route 53 Management Console or API to create, inspect, modify, and delete hosted zones.
