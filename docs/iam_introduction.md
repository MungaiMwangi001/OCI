# Oracle Cloud Infrastructure IAM

IAM stands for **Identity and Access Management service**.

It's also sometimes referred to as:
- **Fine-Grained Access Control**
- **Role-Based Access Control**

There are two key aspects to this service:
- **Authentication (AuthN)**: Who is  someone?
- **Authorization (AuthZ)**: what someone is allowed to do?

- This allows  users to be assigned one or mor predetermined  roles 
- Each  role come with certain permisions?

IAM in OCI consists of Principals, Policies, Federation, and a few other components.

## Identity Domains

An Identity Domain is a container for users and groups.

How does it works ?
1. Create an Identity Doamin
2. Create Users and Groups
3. Write Policies against those groups
4. Policies are scoped to a tenancy/account/compartment
5. Resource area available within a compartment

Each resource in the OCI has its own assigned identifier, which is called **Oracle Cloud ID (OCID)**. Oracle generates these unique identifiers.

The syntax is:

    ocid1.<resource_type>.<realm>.[region][.future_use].<unique_id>

where:

- *resource_type* is kind of the type of the resource (e.g. compute instance, block storage, etc.)
- *realm* is basically set of regions that share the same characteristics (e.g. commercial, government, etc.)
- *region* is the region code
- *unique_id* is the unique identifier of the resource

Examples:

    [Tenancy] ocid1.tenancy.oc1..aaaaartg56hjrtyu84556fdfdtqu56 (NOTE: no region!)
    [Block Volume] ocid1.volume.oc1.eu-frankfurt-1.dsarhsd456hfd98fkajh45as





