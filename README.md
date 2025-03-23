# osTicket Post-Installation Setup

## Overview
This repository documents the post-installation configuration of an osTicket helpdesk system, focusing on roles, departments, teams, agent/user setup, SLA policies, and help topics to ensure an efficient ticketing system.

## Components
- Primary System: Windows 10 (Azure Virtual Machine)
- osTicket Version: 1.15.8
- Database: MySQL 5.5.62

## Steps Taken
1. Accessing osTicket
  - Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
  - End Users osTicket URL: http://localhost/osTicket
2. Configuring Roles (Grouping Permissions)
  - Admin Panel → Agents → Roles
    - Created Role: Supreme Admin
3. Configuring Departments (Ticket Visibility & Categorization)
  - Admin Panel → Agents → Departments
    - Created Department: SysAdmins
4. Configuring Teams (Cross-Departmental Ticket Handling)
  - Admin Panel → Agents → Teams
    - Created Team: Online Banking (Pulls agents from multiple departments)
5. Adjusting Ticket Creation Permissions
  - Admin Panel → Settings → User Settings
    - Unchecked: Unregistered users can create tickets
    - Enabled: Registration Required (Users must register/login to create tickets)
6. Adding Agents (Support Staff)
  - Admin Panel → Agents → Add New
    - Jane (Department: SysAdmins)
    - John (Department: Support)
7. Adding Users (Customers)
  - Agent Panel → Users → Add New
    - Karen
    - Ken
8. Configuring SLA Policies (Service-Level Agreements)
  - Admin Panel → Manage → SLA
    - Sev-A: Grace Period: 1 hour, Schedule: 24/7
    - Sev-B: Grace Period: 4 hours, Schedule: 24/7
    - Sev-C: Grace Period: 8 hours, Schedule: Business Hours
9. Setting Up Help Topics (User Ticket Categories)
  - Admin Panel → Manage → Help Topics
    - Business Critical Outage
    - Personal Computer Issues
    - Equipment Request
    - Password Reset
    - Other

## Verification Screenshots
![Roles](https://github.com/user-attachments/assets/71269b28-f729-4509-8786-766a9444e000)
![Departments](https://github.com/user-attachments/assets/9fcf31f7-e0f6-4442-b0e3-42c4161bc92a)
![Teams](https://github.com/user-attachments/assets/1f217356-2ba8-4229-846c-2b5a965e4c9d)
![Unregistered Users](https://github.com/user-attachments/assets/f939252d-fe36-4c1d-8f24-2ae843c93595)
![Agents](https://github.com/user-attachments/assets/c264afe9-58fb-4b8b-ab92-f14b970f88f5)
![Users](https://github.com/user-attachments/assets/3b5a73ee-c43a-4c5e-a0cb-4bb61aa2578e)
![SLA](https://github.com/user-attachments/assets/9ccb1e00-a0db-4dac-86e1-59c8601cec4c)
![Help Topics](https://github.com/user-attachments/assets/4e7a732f-e0c9-40d7-9246-96607987bb58)









