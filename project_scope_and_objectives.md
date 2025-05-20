# Lucia Finserv HRMS - Project Scope and Objectives

## 1. Project Overview

Lucia Finserv HRMS is a comprehensive financial services management platform designed to streamline operations, enforce role-based access control, and provide tailored experiences for different organizational roles. The system will serve as the central hub for managing employees, branches, client relationships, and business data across the organization.

## 2. Core Objectives

1. **Streamline Organizational Management**: Create a unified platform to manage all aspects of the financial services organization, including employee data, branch operations, and client relationships.

2. **Implement Role-Based Access Control**: Develop a sophisticated permission system that enforces appropriate access levels based on six distinct user roles within the organizational hierarchy.

3. **Enhance Operational Efficiency**: Automate routine tasks such as attendance tracking, leave management, and file/lead assignment to improve productivity and reduce administrative overhead.

4. **Improve Data Visibility**: Provide role-appropriate dashboards and reporting tools that offer insights into business performance, employee activities, and organizational metrics.

5. **Ensure Compliance**: Enforce organizational policies regarding work hours, attendance, and approval workflows through automated system controls.

## 3. Key Features and Functionalities

### 3.1 User Authentication and Access Control
- Secure login system with two-device limitation per user account
- Role-based access control with six distinct user roles
- Role-specific dashboards and navigation experiences

### 3.2 Employee Management
- Employee profiles with comprehensive personal and professional information
- Hierarchical organization structure with departments and teams
- Birthday tracking and notifications
- Employee ID system as a critical identifier

### 3.3 Attendance and Time Management
- Clock-in/clock-out functionality with deadline enforcement (10:30 AM)
- Automatic clock-out at 8 PM if forgotten
- Office hours monitoring (10 AM - 7 PM)
- Attendance reporting and analytics

### 3.4 Leave Management
- Leave request submission and approval workflow
- Secondary approval for certain leave requests
- Leave balance tracking and reporting

### 3.5 Branch Management
- Multi-branch support with branch-specific data segregation
- Branch performance metrics and reporting
- Branch admin capabilities for managing multiple branches

### 3.6 Lead and File Management
- Lead tracking and assignment
- File status monitoring (in progress, opened, closed)
- Strict access controls for viewing and editing leads/files
- Reassignment capabilities for authorized roles

### 3.7 Invoice System
- Invoice generation for opened and closed files
- Invoice download functionality
- File ID as a critical identifier

### 3.8 Notifications
- Push notification system
- Targeted notifications to specific organizational segments
- System alerts for important events and deadlines

### 3.9 Reporting and Analytics
- Comprehensive business data visualization
- Role-appropriate access to organizational metrics
- Performance tracking at individual, team, and branch levels

## 4. User Roles and Permissions

### 4.1 Super Admin
- Highest level of system access
- Branch management capabilities
- Employee oversight across the organization
- Login details visibility
- Role assignment authority
- Secondary approval for leave requests
- Access to all organizational business data
- Birthday tracking across organization
- Office timing management
- Push notification capabilities to all segments

### 4.2 Branch Admin
- Branch head responsibilities
- Multi-branch management capabilities
- Business data visibility across managed branches
- Employee birthday tracking within branches
- Login/logout time monitoring
- Cannot modify attendance records
- No access to technical system modifications

### 4.3 Branch Manager/HR
- Branch-specific HR responsibilities
- Employee management within branch
- Limited access to business data

### 4.4 Team Leader
- Oversight of multiple teams within department
- View team's business data (read-only)
- Must escalate modifications to branch admin or super admin

### 4.5 Employee
- Access to personal leads and files only
- Clock-in/clock-out responsibilities
- Limited system access based on department

### 4.6 Client
- Limited access to personal file information
- Invoice download capabilities for their files

## 5. Technical Requirements

### 5.1 Technology Stack
- Backend: Node.js
- Frontend: Next.js with Chakra UI
- Database: PostgreSQL

### 5.2 System Architecture
- Responsive web application
- Secure API endpoints with proper authentication
- Database design with appropriate relationships and constraints
- Scalable architecture to support organizational growth

### 5.3 Security Requirements
- Secure authentication and authorization
- Data encryption for sensitive information
- Audit logging for critical actions
- Session management with appropriate timeouts

## 6. Project Deliverables

1. Fully functional HRMS platform with all specified features
2. User documentation for each role
3. Administrative documentation for system management
4. Training materials for system adoption
5. Deployment scripts and configuration files
6. Source code with appropriate documentation

## 7. Success Criteria

1. All user roles can access their appropriate functionalities
2. Role-based permissions correctly limit access to authorized features
3. Attendance tracking accurately enforces organizational policies
4. Lead and file management respects access control rules
5. Invoice system correctly generates downloadable documents
6. Notification system delivers targeted messages to appropriate segments
7. System performance meets specified requirements under expected load
8. User interface is intuitive and responsive across devices
