
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
