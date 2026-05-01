
## EC2 — Advanced Settings
1. Stop Protection
Protects the instance against accidental stops. Must be manually disabled before stopping.

2. Detailed CloudWatch Monitoring

Disabled → metrics every 5 minutes (free)
Enabled → metrics every 1 minute (additional cost)


3. Credit Specification
    Only for T family instances (t2, t3...).

Standard → uses CPU credits and stops when they run out
Unlimited → keeps running even without credits, but charges extra ⚠️


4. Placement Group
Defines how instances are physically distributed across data centers:

Cluster → low latency, same rack
Spread → instances on separate racks
Partition → isolated groups for big data


5. EBS-Optimized Instance
Guarantees dedicated bandwidth between the instance and EBS storage, improving disk performance.

6. Instance Bandwidth Configuration
Configures the instance's network bandwidth to optimize data transfer performance.

7. Purchasing Option
Defines how you pay for the instance:

None → On-Demand (default, pay per use)
Capacity Blocks → reserves capacity for specific workloads
Spot Instances → instances with up to 90% discount, but can be interrupted by AWS ⚠️


8. Capacity Reservation
Reserves capacity in a specific AZ to ensure your instance always has resources available, even during high demand periods.


💡 Tip: For production use On-Demand or Reserved. For flexible and fault-tolerant workloads, use Spot Instances to save money! 🚀

---

🖼️ AMI — Amazon Machine Image
Think of an AMI as a "template" or "snapshot" of your server. It's like a complete photo of an already configured system.

📀 ISO Analogy
As you mentioned, it's similar to an ISO — but goes further:
Traditional ISOAMIClean operating systemOS + applications + configurationsNeed to install everything from scratchAlready ready to useUsed onceCan launch multiple instances

📦 What does an AMI contain?

Operating system (Linux, Windows, etc.)
Pre-installed software (Node, Nginx, Python...)
System configurations
Initial data if needed


🔄 Types of AMI

AWS official → Amazon Linux, Ubuntu, Windows Server
AWS Marketplace → ready-made AMIs from third parties (ex: WordPress, etc.)
Custom → you create your own from a configured instance
Community → created by the community, free of charge


💡 Practical Example
Imagine you configured a server with:

Node.js installed
Nginx configured
Your application running

You can create an AMI from that server and use it to launch 10 identical instances in seconds! 🚀

⚠️ Important: AMIs are regional — if you create one in São Paulo, you need to copy it to use in another region!

---
⚖️ Load Balancers
A Load Balancer is a traffic distributor — it receives requests and distributes them across multiple instances, preventing any single server from being overloaded.

🔄 How it works
Users → Load Balancer → Instance 1
                      → Instance 2
                      → Instance 3

📦 Types of Load Balancers on AWS

ALB (Application Load Balancer)

Works at Layer 7 (HTTP/HTTPS)
Routes traffic based on URL, headers, cookies
Best for web applications and APIs


NLB (Network Load Balancer)

Works at Layer 4 (TCP/UDP)
Extremely high performance and low latency
Best for real-time applications


GLB (Gateway Load Balancer)

Used for security and firewall appliances
Routes traffic through third-party virtual appliances


CLB (Classic Load Balancer)

Legacy — old generation
Not recommended for new projects ⚠️




✅ Main Benefits

High availability — if one instance fails, traffic goes to another
Scalability — distributes load automatically
Health checks — removes unhealthy instances automatically
SSL termination — manages HTTPS certificates centrally


💡 Practical Example
Imagine your app has 3 EC2 instances. Without a Load Balancer, all traffic hits just one server. With a Load Balancer:

Instance 1 → handles 33% of traffic
Instance 2 → handles 33% of traffic
Instance 3 → handles 33% of traffic

If Instance 1 goes down → Load Balancer automatically redirects to Instances 2 and 3! 🚀


💡 Tip: For most web applications, ALB is the best choice. Use NLB only when you need ultra-low latency! ⚡
