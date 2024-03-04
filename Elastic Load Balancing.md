You can configure health checks, which monitor the health of the compute resources, so that the load balancer sends requests only to the healthy ones.


Elastic Load Balancing supports the following types of load balancers: 
• Application Load Balancers 
• Network Load Balancers 
• Gateway Load Balancers 
• Classic Load Balancers

When you enable an Availability Zone for your load balancer, Elastic Load Balancing creates a load balancer node in the Availability Zone

The nodes for your load balancer distribute requests from clients to registered targets. When crosszone load balancing is enabled, each load balancer node distributes traffic across the registered targets in all enabled Availability Zones. When cross-zone load balancing is disabled, each load balancer node distributes traffic only across the registered targets in its Availability Zone
![[Pasted image 20240123123929.png]]