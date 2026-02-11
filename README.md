## AWS Cost Savings

### AWS Promotional Credits

AWS provides promotional credits to startups, enterprises, and customers running proof-of-concepts or migrations.

* Credits can be used to pay for most AWS services.
* They usually expire in 12 months.
* Startups can receive between $1,000 and $100,000 depending on program and funding stage.

Why it saves money:

* Credits directly reduce your AWS bill.
* They allow you to experiment, scale, and optimize before spending real cash.

When to use:

* Early-stage startups
* New workloads
* Cloud migrations or pilots

---

### Using Private IPs Instead of Elastic IPs

Elastic IPs cause traffic to route through public infrastructure, even inside AWS.

* Private IP communication inside the same VPC is cheaper.
* Inter-AZ data transfer costs apply when traffic crosses Availability Zones.

Why it saves money:

* Avoids public data transfer charges.
* Reduces inter-AZ data transfer costs.

When to use:

* Internal service-to-service communication
* Backend microservices
* Databases and application servers

---

### Spot Instances for Compute Savings

Spot Instances use unused AWS capacity at a steep discount.

* Prices are up to 90% cheaper than On-Demand instances.
* Instances can be interrupted by AWS with short notice.

Why it saves money:

* You pay a fraction of normal compute cost.

When to use:

* Batch jobs
* CI/CD pipelines
* Data processing
* Stateless or fault-tolerant workloads

---

### Reserved Instances from AWS Marketplace

Reserved Instances commit you to long-term usage.

* Marketplace Reserved Instances are often cheaper than standard AWS Reserved Instances.
* Commitments are typically 1 or 3 years.

Why it saves money:

* Savings of up to 75% compared to On-Demand pricing.

When to use:

* Steady, predictable workloads
* Always-on production systems

---

### Reserved ElastiCache Nodes

ElastiCache is commonly used for Redis or Memcached.

* Reserved nodes provide large discounts for long-term usage.

Why it saves money:

* Up to 77% discount compared to On-Demand nodes.

When to use:

* Persistent caching layers
* Session storage
* High-throughput applications

---

### Using S3 for Backups Instead of EBS

EBS volumes are expensive for long-term storage.
Amazon S3 is designed for durable, low-cost storage.

Why it saves money:

* S3 storage is significantly cheaper than EBS.
* Lifecycle rules can move data to even cheaper tiers.

When to use:

* Backups
* Logs
* Archives and snapshots

---

### Upgrading to New Generation EC2 Instance Families

Newer EC2 families offer better performance per dollar.

* Better CPUs
* More efficient networking
* Improved memory bandwidth

Why it saves money:

* The same workload runs faster on fewer resources.
* Savings of up to 20%.

When to use:

* Legacy instances
* Long-running applications

---

### Auto Scaling for Idle Resources

Many instances run underutilized or idle.

* Auto Scaling adjusts capacity based on demand.
* Instances are removed when traffic drops.

Why it saves money:

* You only pay for resources you actually use.

When to use:

* Variable traffic workloads
* APIs and web applications
* Background processing systems

---

### Selecting Cost-Effective AWS Regions

AWS pricing varies by region.

* North Virginia (us-east-1) is one of the cheapest regions.
* Regions like São Paulo are significantly more expensive.

Why it saves money:

* Lower EC2, storage, and data transfer pricing.

When to use:

* Non-regulated workloads
* Systems without strict latency requirements

---

### Reducing Data Transfer with GraphQL APIs

REST APIs often return more data than required.
GraphQL allows clients to request only the exact data they need.

Why it saves money:

* Smaller payloads mean less outbound data transfer.
* Fewer API calls are required.

When to use:

* Mobile applications
* Bandwidth-sensitive systems
* Public APIs with high traffic

---

### Using CloudFront for Data Transfer

Data transfer from AWS to the internet is expensive.
CloudFront is AWS’s CDN that caches content closer to users.

* CloudFront data transfer rates are much cheaper than direct EC2 or ALB outbound traffic.
* It reduces load on origin servers.

Why it saves money:

* Outbound traffic via CloudFront can be up to 75% cheaper.
* Cached content reduces repeated requests to backend services.

When to use:

* Web applications
* APIs with global users
* Static and media-heavy workloads

---

### Using S3 VPC Endpoints and Enhanced Networking

S3 VPC Endpoints allow private traffic between EC2 and S3.
Enhanced Networking improves throughput and latency.

Why it saves money:

* Eliminates NAT Gateway and public data transfer charges.
* Improves performance without scaling up instance size.

When to use:

* Heavy S3 usage
* High-performance workloads

---

### Removing Idle Load Balancers

Load Balancers are billed hourly, even if unused.

Why it saves money:

* Eliminates unnecessary fixed costs.

When to use:

* After migrations
* After testing or environment cleanup

---

### AWS Savings Plans

Savings Plans offer flexible discounts across AWS services.

* Applies to EC2, Fargate, and Lambda.
* Automatically applies to eligible usage.

Why it saves money:

* Up to 72% discount compared to On-Demand pricing.

When to use:

* Consistent usage patterns
* Mixed compute environments

