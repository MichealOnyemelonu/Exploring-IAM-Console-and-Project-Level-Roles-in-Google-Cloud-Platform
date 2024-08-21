# Exploring-IAM-Console-and-Project-Level-Roles-in-Google-Cloud-Platform

## Overview

This project is part of my exploration of the Identity and Access Management (IAM) console in Google Cloud Platform (GCP). The focus is on understanding project-level roles and how they affect access to resources within a GCP project. The tasks involved include assigning roles, creating a Cloud Storage bucket, managing access, and verifying permissions.

## Tasks and Steps

### Task 1: Explore the IAM Console and Project-Level Roles

1. **Accessing the IAM Console**
   - Navigated to the IAM & Admin section in the GCP Console.
   - Explored the basic roles: **Viewer**, **Editor**, and **Owner**.
   - These roles determine the level of access and control a user has over GCP services in a project.

2. **Assigning and Exploring Roles**
   - Two user accounts were used: **Username 1** (Project Owner) and **Username 2** (Project Viewer).
   - Verified the permissions associated with each role, particularly noting the limitations of the Viewer role compared to the Owner.

### Task 2: Prepare a Cloud Storage Bucket for Access Testing

1. **Creating a Cloud Storage Bucket**
   - Created a new Cloud Storage bucket with a unique name.
   - Configured the bucket with a Multi-Region location type.

2. **Uploading a Sample File**
   - Uploaded a file named `sample.txt` to the bucket to test access permissions.
   - Verified that the Viewer role could only view the file without making modifications.

3. **Verifying Access for Username 2**
   - Checked that **Username 2** could view the bucket and the `sample.txt` file, confirming the read-only permissions of the Viewer role.

### Task 3: Remove Project Access

1. **Removing Project Viewer Role from Username 2**
   - Revoked the Viewer role from **Username 2** using **Username 1**.
   - Verified that **Username 2** no longer had access to the project resources.

2. **Verifying Access Removal**
   - Attempted to access the Cloud Storage bucket with **Username 2** post-revocation and received a permission error, confirming the removal.

## Key Learnings

- **Role Management:** Understanding the assignment and revocation of roles within GCP.
- **Permissions Impact:** Observing how different roles influence user actions.
- **Security Practices:** Managing and revoking access securely in a cloud environment.

## Conclusion

This project showcases my ability to manage IAM roles within Google Cloud Platform, ensuring secure and appropriate access to resources. It highlights essential skills needed for cloud security and administration roles.

## Repository Structure

- `README.md`: Project overview and details.
- `images/`: (Optional) Directory for screenshots related to the project.

