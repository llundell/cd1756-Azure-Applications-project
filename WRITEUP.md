# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### App Service
- **Cost:** Lowered total cost since Microsoft manages the underlying infrastructure and you pay for the capacity required, not the servers.
- **Scalability:** App Service also provides auto-scaling to support greater demand on CPU or memory as needed so no manual capacity planning is needed. 
- **Availability:** It's highly available by design, reducing the risk of downtime due built-in redundancy
- **Workflow:** It's faster to set up and maintain an App Service as it can be deployed in a few minutes with minimal configuration and doesn't require OS configuration.
 
### Virtual Machine
- **Cost:** VMs can be more cost effective in the long-term when steady workloads are expcted, though there is a higher operational costs since Azure doesn't manage the OS.
- **Scalability:** Scaling is manual could require additional tools to manage so it's a better choice for predictible size needs.
- **Availability:** There is the option for high availability but it must be designed that way, vs the App Service which provides high availability by default.
- **Workflow:** Full control of the OS is provided so best used for legacy applications or custom system-level configuration needs.
 
### My Choice & Justification

I chose the App Service over Virtual Machine for this specific app because it lowers the total cost since Microsoft manages the underlying infrastructure. App Service also provides auto-scaling to support greater demand on CPU or memory as needed so as the app grew, it could be scaled automatically. It's highly available by design, reducing the risk of downtime due built-in redundancy. It's faster to set up and maintain an App Service as it can be deployed in a few minutes with minimal configuration and doesn't require OS configuration. Also, the workload is web-based so doesn't require system-level control. 

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

If I began to add additional apps that needed to interact with one another, that would be a good use case for using a VM. Also, if any custom configurations were needed on the OS, that would require a VM. If there were any special networking or security requirements like custom firewall rules, an App Service would be unable to provide those so a VM would be necessary. 
