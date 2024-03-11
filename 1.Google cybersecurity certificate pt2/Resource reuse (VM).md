When a [[hypervisor]] Reuses resources between different VMs resulting in the inadvertent sharing of data between VMs 

e.g. sharing 4gb between 3 VMs with 2gb each, the system doesn't have 6gb therefore the hypervisor may overlap memory between different VMs

- Not common: well-built hypervisors effectively isolate between VMs and employ mechanisms to avoid resource reuse