- Azure accounts
- subscriptions - resources
- most of the time a temporary subscription is created for you, which runs in an environment called the Learn sandbox.
- Azure free account
- Azure free student account - 12 months
- Microsoft learn sanbox

### Bash Commands
- date: command to get the current date and time
- az upgrade: run an update to the CLI
- pwsh: to change back to PowerShell mode
- az interactive: Interactive mode provides autocompletion, command descriptions, and even examples


### Azure Physical Infrastructure
1. Datacenters: resources arranged in racks, with dedicated power, cooling, and networking infrastructure
    - Datacenters are grouped into Azure Regions or Azure Availability Zones
    - Region: A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network
    - Availability Zones: physically separate datacenters within an Azure region
    - An availability zone is set up to be an isolation boundary. If one zone goes down, the other continues working. Availability zones are connected through high-speed, private fiber-optic networks.
      

Azure services that support availability zones fall into three categories:

- Zonal services: You pin the resource to a specific zone (for example, VMs, managed disks, IP addresses).
- Zone-redundant services: The platform replicates automatically across zones (for example, zone-redundant storage, SQL Database).
- Non-regional services: Services are always available from Azure geographies and are resilient to zone-wide outages as well as region-wide outages.

### Region Pairs
- regions are paired with another region within the same geography at least 300 miles away
- allows for the replication of resources across a geography that helps reduce the likelihood of interruptions because of events such as natural disasters, civil unrest, power outages, or physical network outages that affect an entire region
- recovery and replication must be configured by the customer
- Examples of region pairs in Azure are West US paired with East US and South-East Asia paired with East Asia
- provide reliable services and data redundancy
- Most regions are paired in two directions, meaning they are the backup for the region that provides a backup for them
- updates are rolled out to paired regions one region at a time to minimize downtime and risk of application outage

### Sovereign Regions
- instances of Azure that are isolated from the main instance of Azure
- use a sovereign region for compliance or legal purposes
- Ex. US DoD Central, US Gov Virginia, US Gov Iowa
