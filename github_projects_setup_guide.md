# GitHub Projects Setup Guide for Lucia Finserv HRMS

This guide provides step-by-step instructions for setting up GitHub Projects as the project management tool for the Lucia Finserv HRMS project.

## Why GitHub Projects?

GitHub Projects offers several advantages for our project:

1. **Seamless Integration**: Direct connection with our GitHub repository
2. **Simplified Workflow**: Issues and pull requests automatically appear in the project board
3. **Visibility**: Team members can see both code and project management in one place
4. **Cost-Effective**: Included with GitHub, no additional subscription needed
5. **Familiar Interface**: Developers already using GitHub will find it intuitive

## Setup Instructions

### 1. Create a Project Board

1. Navigate to the [Lucia HRMS repository](https://github.com/manoj-lucia/lucia_hrms)
2. Click on the "Projects" tab
3. Click "New project"
4. Select "Board" as the template
5. Name the project "Lucia Finserv HRMS Development"
6. Add a brief description: "Project management board for Lucia Finserv HRMS development"
7. Click "Create"

### 2. Configure Project Columns

The default board comes with "Todo", "In Progress", and "Done" columns. Let's customize it for our development workflow:

1. Click "+" to add more columns
2. Set up the following columns:
   - **Backlog**: Tasks that are defined but not yet ready for development
   - **Ready for Development**: Tasks that are fully specified and ready to be worked on
   - **In Progress**: Tasks currently being worked on
   - **Code Review**: Tasks with pull requests awaiting review
   - **Testing**: Tasks that are implemented but need testing
   - **Done**: Completed tasks

3. For each column, click the "..." menu and select "Manage automation" to set up automatic card movement:
   - **In Progress**: Move issues here when assigned or when a branch is created
   - **Code Review**: Move issues here when a pull request is opened
   - **Done**: Move issues here when pull requests are merged

### 3. Create Issue Templates

1. In the repository, create a `.github/ISSUE_TEMPLATE` directory
2. Create the following template files:

#### Feature Request Template (feature_request.md):
```markdown
---
name: Feature request
about: Suggest a feature for the Lucia Finserv HRMS
title: '[FEATURE] '
labels: enhancement
assignees: ''
---

## Feature Description
A clear and concise description of the feature.

## User Story
As a [role], I want [feature] so that [benefit].

## Acceptance Criteria
- [ ] Criterion 1
- [ ] Criterion 2
- [ ] Criterion 3

## Additional Context
Add any other context, mockups, or screenshots about the feature request here.
```

#### Bug Report Template (bug_report.md):
```markdown
---
name: Bug report
about: Report a bug in the Lucia Finserv HRMS
title: '[BUG] '
labels: bug
assignees: ''
---

## Bug Description
A clear and concise description of the bug.

## Steps to Reproduce
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

## Expected Behavior
A clear and concise description of what you expected to happen.

## Screenshots
If applicable, add screenshots to help explain your problem.

## Environment
- Device: [e.g. Desktop, iPhone 12]
- OS: [e.g. Windows 10, iOS 14]
- Browser: [e.g. Chrome 91, Safari 14]
- Version: [e.g. 1.0.0]

## Additional Context
Add any other context about the problem here.
```

### 4. Set Up Labels

Create the following labels to categorize issues:

1. Navigate to Issues → Labels → New Label
2. Create these labels:
   - `bug`: Bug reports
   - `enhancement`: Feature requests
   - `documentation`: Documentation updates
   - `frontend`: Frontend-related tasks
   - `backend`: Backend-related tasks
   - `database`: Database-related tasks
   - `ui/ux`: User interface and experience tasks
   - `high-priority`: Urgent tasks
   - `medium-priority`: Normal priority tasks
   - `low-priority`: Tasks that can wait
   - `role:client`: Features related to client role
   - `role:employee`: Features related to employee role
   - `role:team-leader`: Features related to team leader role
   - `role:branch-admin`: Features related to branch admin role
   - `role:branch-manager`: Features related to branch manager role
   - `role:super-admin`: Features related to super admin role

### 5. Create Initial Milestones

1. Navigate to Issues → Milestones → New Milestone
2. Create the following milestones:
   - **Project Setup**: Initial repository and environment setup
   - **Core Architecture**: Basic application architecture and infrastructure
   - **Authentication System**: User authentication and role-based access control
   - **Employee Management**: Employee profiles and management features
   - **Branch Management**: Branch creation and management features
   - **Attendance System**: Clock-in/clock-out functionality
   - **Leave Management**: Leave request and approval system
   - **File/Lead Management**: Client file and lead tracking
   - **Invoice System**: Invoice generation and management
   - **Reporting Dashboard**: Analytics and reporting features
   - **Beta Release**: Feature-complete version for testing
   - **Production Release**: Final version ready for deployment

### 6. Create Initial Project Tasks

Create issues for the initial project setup phase:

1. Repository structure setup
2. Development environment configuration
3. Database schema design
4. API architecture planning
5. UI/UX wireframing
6. Authentication system design
7. Role-based access control implementation plan

### 7. Set Up Project Workflow

1. **Weekly Planning**:
   - Review the backlog
   - Move items to "Ready for Development"
   - Assign tasks to team members

2. **Daily Updates**:
   - Team members update their assigned issues
   - Move cards across the board as work progresses

3. **Code Review Process**:
   - Pull requests linked to issues
   - Reviewers assigned to pull requests
   - Issues move to "Testing" after approval

4. **Completion**:
   - Issues closed when fully implemented and tested
   - Milestone progress tracked

## Best Practices

1. **Link Pull Requests to Issues**: Use keywords like "Fixes #123" or "Closes #123" in pull request descriptions to automatically link them to issues.

2. **Use Issue References**: When committing code, reference the issue number (e.g., "Add login form #42").

3. **Keep the Board Updated**: Move cards to reflect the current status of work.

4. **Regular Cleanup**: Periodically review and update the board to keep it relevant.

5. **Use Milestones**: Track progress toward major project phases.

## Additional Resources

- [GitHub Projects Documentation](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects)
- [GitHub Issues Documentation](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)
- [GitHub Pull Requests Documentation](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
