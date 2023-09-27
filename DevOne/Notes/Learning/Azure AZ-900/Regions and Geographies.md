A **region** is a grouping of multiple data-centers.

- Azure has 58 regions across 140 countries.

A **geography** is a discreet market of two or more regions that preserves data residency and compliance boundaries.

- Azure relies on paired regions for disaster recovery, only one region is updated at a time so this ensures that there are no outages.

# Region Types and Service Availability

### **Recommended Region**

A region that provides the broadest range of service capabilities and designed to support Availability Zones now or in the future.

### **Alternate region**

A region that extends Azure’s footprint within a data residency boundary where a recommended region also exists.

Not designed to support **Availability Zones**.

These regions are labeled as Other.

### General Availability

Is when a service is considered ready to be used publicly by everyone.

# Azure Cloud Services

ACS are grouped in three categories, their category determines when cloud services become available.

1. Foundational.
    1. When GA, immediately or in 12 months in Recommended and Alternate Regions.
2. Mainstream.
    1. When GA, immediately or in 12 months in Recommended Regions.
    2. May become available in Alternate Regions based on customer demand.
3. Specialized
    1. Available in Recommended or Alternate Regions based on customer demand.

# Special Regions

Azure has specialized regions to meet compliance or legal reasons.

# Availability Zones

Are physical locations made up of one or more data centers.

A data center is a secured building that contains hundreds of thousands of computers.

A region will generally contain 3 availability zones.

Data centers within a region will be isolated from each other, but close enough to provide low latency.

## Supported regions

Not every region has support for AZs, these regions are known as Alternate and Other.

**Recommended regions are supposed to have at least 3 AZs**.

# Fault and Update domains

An AZ is a combination of a fault domain and an update domain.

### Fault Domain

A logical grouping of hardware to avoid a single point of failure within an AZ.

### Update Domain

Azure may need to apply updates to the underlying hardware and software, update domains ensure your resources don’t go offline.

### Availability Set

A logical grouping that you can use in Azure to ensure that the VMs you place in the Availability Set are different fault/update domains to avoid downtime.