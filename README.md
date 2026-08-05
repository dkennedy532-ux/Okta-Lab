# Okta-Lab

# Description
Hands on Okta IAM lab demonstrating user provisioning, group-based access control, MFA, application assignment, and the identity lifecycle

# Tools Used
- Okta Integrator Free Plan
- Okta Universal Directory
- Okta Authentication Policies
- Okta Application Assignments

# Skills Developed and Learned
- Identity and Access Management
- Okta Administration
- User Provisioning
- Group Management
- Role-Based Access Control
- Application Assignment
- Multi-Factor Authentication
- Identity Lifecycle Management
- User Deprovisioning
- Least Privilege
- Access Troubleshooting

# 1: Create Department Groups
<img width="1433" height="818" alt="Create Groups" src="https://github.com/user-attachments/assets/0fd32bfd-dc32-494e-a453-49b1e9b7d80a" />
Created different groups to provide scalable way to demonstrate group based access

# 2: Create Employee Accounts
<img width="1440" height="821" alt="Create Employees" src="https://github.com/user-attachments/assets/3e795e3e-e985-49fd-b02a-cccd27e0662b" />
I created fake employee identities and assigned each user to the appropriate department group

# 3: Configure Group Based Applications
<img width="1440" height="822" alt="App Configuration" src="https://github.com/user-attachments/assets/a9409fc1-8e72-4bf2-9763-08ae7e90b795" />
I assigned the Zoom application to the HR group.
The application was assigned to the group rather than directly to the employee to demonstrate Role Based Access Control 

# 4: Verify Access
<img width="1440" height="821" alt="Verify Access" src="https://github.com/user-attachments/assets/6051e318-c081-426c-8c4d-0fd96c0344ba" />
I verified that the employee received access to the assigned application because she was a member of the Human Resources group. This confirmed that access was inherited through group membership rather than through user assignment

# 5: Group Transfer
<img width="1438" height="822" alt="Group Transfer" src="https://github.com/user-attachments/assets/91695273-1263-43ff-8fb4-38c6f5f563a2" />
To demonstrate the mover stage of the identity lifecycle I transferred her from HR to Finance.I removed her from the HR group and added her to the Finance group.This represents how an IAM administrator updates access when an employee changes roles or departments.

# 6: MFA
<img width="1440" height="820" alt="MFA" src="https://github.com/user-attachments/assets/301aac5e-79d0-4b8a-bca1-58d018e7b4b1" />
I reviewed and configured an application sign in policy requiring two authentication factors

# 7: Deactivate
<img width="1436" height="817" alt="Deactivate" src="https://github.com/user-attachments/assets/b4a0fc02-e448-4c4b-a953-1ec4efe7d51e" />
Deactivation prevents the user from signing in and helps revoke access to organizational applications after employment ends

# Security Principles Demonstrated
- Role Based Access Control
- Access was assigned using department groups instead of direct user assignment
- Least Privilege
- Users received access based on their job function and group membership
- Multi-Factor Authentication
- Centralized Identity Management

# Help Desk Scenario
# A user reports that the Zoom application does not appear on their Okta dashboard.
- Confirm that the user account is active
- Verify the user's department group membership
- Confirm that Zoom is assigned to the correct group
- Review the application's sign on policy
- Verify that the user has completed required MFA enrollment
# Resolution
Correct the user's group membership or application assignment and verify that the application becomes available

# Lessons Learned
This lab showed how Okta can centralize identity administration and application access. 
I learned that assigning applications through groups makes onboarding, department transfers, and offboarding more efficient. I also practiced enforcing MFA and managing access throughout the employee identity lifecycle









