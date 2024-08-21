# GCP IAM Role Exploration

## Overview

This repository contains a project focused on exploring Identity and Access Management (IAM) roles in Google Cloud Platform (GCP). It demonstrates how different project-level roles, such as Viewer, Editor, and Owner, affect permissions and access to resources.

## Contents

- **Task 1: Explore the IAM Console and Project-Level Roles**
  - Navigating the IAM console.
  - Assigning roles and observing permissions.
  
- **Task 2: Prepare a Cloud Storage Bucket for Access Testing**
  - Creating a Cloud Storage bucket.
  - Testing access with different IAM roles.
  - Revoking and verifying access.

## Key Learnings

- Understanding GCP IAM roles and their impact on project permissions.
- Practical experience in managing and revoking access.
- Security best practices in cloud environments.

## Repository Structure

- `README.md`: This file, providing an overview of the project.
- `images/`: Contains screenshots related to the project (e.g., IAM console, role assignment).
- `tasks/`: Detailed markdown files for each task, explaining the steps taken and results observed.

## How to Use

1. **Task Documentation**: Navigate to the `tasks/` directory for detailed documentation of each task.
2. **Screenshots**: Visual references are available in the `images/` directory.

## Conclusion

This project showcases the ability to manage IAM roles within Google Cloud Platform, which is essential for cloud security and administration roles.

# Task 1: Explore the IAM Console and Project-Level Roles

## Steps Taken

1. **Accessing the IAM Console**
   - Navigated to the IAM & Admin section in GCP Console.
   - Explored roles: Viewer, Editor, Owner.
   - Documented the permissions associated with each role.

2. **Role Assignment and Permissions**
   - Assigned Viewer role to Username 2.
   - Verified that Username 2 could only view resources, not modify them.

## Observations

- **Viewer Role**: Allows read-only access.
- **Editor Role**: Allows modification of existing resources.
- **Owner Role**: Full access, including billing and role management.

## Screenshots

- ![IAM Console](../images/iam-console.png)
- ![Role Assignment](../images/role-assignment.png)
