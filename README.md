# Azure-Project-Identity
Implementing Role-Based Access Control (Identity)

The main objective of this project is to implement Role-Based Access Control (RBAC) in Azure to ensure secure and granular management of resource permissions. By assigning roles to specific users or groups, RBAC enables organisations to enforce the principle of least privilege, allowing users to perform only the tasks they are authorised for without exposing unnecessary access to critical resources.

For example

Job Specific Scenario: Managing Access for a Temporary Consultant

Our organisation has hired a temporary consultant to analyse data stored in Azure Blob Storage. The consultant needs access to upload and manage blob files but should not have full administrative privileges over the storage account or any unrelated Azure resources.

Steps taken:

Add the Consultant as a New User:
Create an user account for the consultant in Azure Active Directory and provide login credentials, ensuring the consultant can securely access Azure resources.

Assign a Role:
To ensure the consultant has appropriate permissions, I've assigned the Storage Blob Contributor role to the consultant for the specific storage account. This allows the consultant to read, upload and delete blobs but prevents access to other resources or critical account settings.

Test Permissions:
Before handing off the account to the consultant, I've tested the access to confirm the role assignment is functioning as intended. The consultant can access the blob storage to upload and manage files but cannot make changes outside their scope.

Audit Activities:
During the consultant’s engagement, I've regularly checked the Sign-ins and Activity Logs in Azure Active Directory to monitor access and ensure compliance with company policies.

Revoke Access Post-Engagement:
Once the consultant's work is complete, I've removed the role assignment and disabled the account to prevent further access.

Outcome: By using RBAC, our organisation ensures that the consultant has only the permissions needed for their tasks, mitigating risks while maintaining operational efficiency. 

This approach aligns with security best practices and regulatory compliance requirements.
