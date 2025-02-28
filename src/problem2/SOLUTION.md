Provide your solution here:
### Frontend
#### Components
![image] (./frontend.png)
* Cloudfront: global CND reduces latency for users
* S3: Store static website files
* Route53: Route traffic to Cloudfront
* Certificate Manager: SSL certificate for Cloudfront
### Backend
#### Components
![image] (./backend.png)
* AWS Global Accelerator: Improve global performance, availability, and security for applications
* AWS ALB: Load balancer for the backend, deployed multiple regions along with eks services
* AWS EKS: Managed Kubernetes service, deployed in multiple regions
* AWS Aurora Global Database: Postgresql database, with read replicas in different regions and automatic failover
* AWS Route53: Route traffic to ALB, Perform health checks and failover to healthy regions
