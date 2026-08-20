# Azure Resource Hierarchy

## What is Resource Hierarchy?
Azure resource hierarchy is the organizational structure used to arrange and manage Azure resources.
It allows organizations to apply policies, access controls, billing, and management at different levels.
The hierarchy consists of:
- Management Groups
- Subscriptions
- Resource Groups
- Resources

## Management Groups
Management groups are used to organize and manage multiple Azure subscriptions.
They allow organizations to apply policies and Role-Based Access Control (RBAC) across multiple subscriptions from a higher level.

**Key points:**
- Can contain multiple subscriptions.
- Policies can be applied across subscriptions.
- RBAC can be managed at this level.
- Provides centralized governance.

## Subscriptions
A subscription provides a boundary for Azure resources and is also associated with billing.

**Key points:**
- Contains resource groups.
- Provides a billing boundary.
- Helps separate environments, departments, or projects.
- Access and policies can be applied at the subscription level.

## Resource Groups
A resource group is a logical container that groups related Azure resources together.
Resources within a resource group can be managed together based on the needs of an application, project, or workload.

**Key points:**
- Groups related resources.
- Helps organize and manage resources.
- Resources can be deployed and managed together.
- Resource groups can have access controls and policies applied to them.

## Resources
Resources are the actual Azure services and components that you create and use.
Examples include:
- Virtual machines (VMs)
- Storage accounts
- Databases
- Virtual networks
- Web applications

# Azure Resource Manager (ARM)
Azure Resource Manager (ARM) is the management layer of Azure. It provides a consistent way to create, manage, update, and delete resources.
When you perform management operations through the Azure portal, Azure CLI, PowerShell, or other Azure management tools, the requests are handled through Azure Resource Manager.

### ARM enables actions such as:
- Deploying and updating resources.
- Deleting resources and resource groups.
- Adding and managing tags.
- Defining infrastructure through templates.
- Controlling access using Role-Based Access Control (RBAC).
- Enforcing organizational policies.
- Applying resource locks to help prevent accidental changes or deletion.

## Best Practices
- Group resources according to their lifecycle.
- Use consistent naming conventions.
- Apply tags to improve organization and management.
- Use resource locks for critical or production resources to help prevent accidental deletion.
- Organize subscriptions and resource groups according to projects, environments, departments, or workloads.

## Key Takeaway
  Azure Resource Hierarchy provides a structured way to organize and govern Azure resources.
  Management Groups sit at the highest level, followed by Subscriptions, Resource Groups, and finally individual Resources.
  Azure Resource Manager provides the management layer through which these resources can be deployed, configured, and controlled.
