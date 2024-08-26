# Google Cloud IAM and Cloud Storage Project

This repository documents tasks performed in Google Cloud IAM and Cloud Storage, including exploring IAM roles, managing Cloud Storage buckets, and configuring access permissions.

## Table of Contents

1. [Exploring IAM Roles](#exploring-iam-roles)
2. [Preparing a Cloud Storage Bucket for Access Testing](#preparing-a-cloud-storage-bucket-for-access-testing)
3. [Removing Project Access](#removing-project-access)
4. [Adding Cloud Storage Permissions](#adding-cloud-storage-permissions)
5. [Verification Steps](#verification-steps)

---

## Exploring IAM Roles

### Task 1: Explore the IAM Console and Project Level Roles

1. **Navigate to IAM Console**:
   - Go to Navigation menu > IAM & Admin > IAM.

2. **Grant Access**:
   - Click the `+GRANT ACCESS` button.
   - Scroll to the "Basic" section under Select a role.
   - Hover over the roles: Editor, Owner, and Viewer.

3. **Role Definitions**:
   - **Viewer** (`roles/viewer`): Read-only access.
   - **Editor** (`roles/editor`): Includes Viewer permissions plus permissions to modify resources.
   - **Owner** (`roles/owner`): Includes Editor permissions plus the ability to manage roles and permissions, and set up billing.

4. **Cancel**:
   - Click `CANCEL` to exit the "Add principal" panel.

---

## Preparing a Cloud Storage Bucket for Access Testing

### Task 2: Create a Bucket and Upload a Sample File

1. **Create a Bucket**:
   - Navigate to Navigation menu > Cloud Storage > Buckets.
   - Click `+CREATE`.
   - Enter a unique name for the bucket and click `CONTINUE`.
   - Set Location Type to "Multi-Region".
   - Click `CREATE`.
   - Confirm if prompted about Public access.

2. **Upload a Sample File**:
   - Go to the Bucket Details page and click `UPLOAD FILES`.
   - Choose a file from your computer and upload it.
   - Rename the file to `sample.txt` by clicking on the three dots next to the file name and selecting `Rename`.

3. **Verify Bucket Creation**:
   - Confirm that the file appears in the bucket.

---

## Removing Project Access

### Task 3: Remove Project Viewer for Username 2

1. **Remove Access**:
   - Navigate to IAM & Admin > IAM.
   - Find Username 2 in the list.
   - Click the pencil icon next to Username 2’s role.
   - Click the trashcan icon next to the Viewer role and then `SAVE`.

2. **Verify Access Removal**:
   - Switch to Username 2 console.
   - Navigate to Cloud Storage and attempt to access the bucket.
   - You should see a permission error indicating that access has been revoked.

---

## Adding Cloud Storage Permissions

### Task 4: Add Cloud Storage Permissions

1. **Grant Cloud Storage Access**:
   - Go back to Username 1 console.
   - Navigate to IAM & Admin > IAM.
   - Click `+GRANT ACCESS`.
   - Enter Username 2 in the New principals field.
   - Select `Cloud Storage > Storage Object Viewer` from the Select a role dropdown.
   - Click `SAVE`.

2. **Verify Cloud Storage Access**:
   - Switch to Username 2 console.
   - Open Cloud Shell and run:
     ```sh
     gsutil ls gs://[YOUR_BUCKET_NAME]
     ```
   - Replace `[YOUR_BUCKET_NAME]` with the bucket name created earlier.
   - You should see the output with the path to `sample.txt`.

---

## Verification Steps

To verify the setup:

1. **Ensure IAM Roles**: Check that Username 2 has the correct permissions.
2. **Cloud Storage Visibility**: Confirm that Username 2 can view the bucket and file as per the `Storage Object Viewer` role.
3. **Access Errors**: Make sure that Username 2 receives a permission error if their access is removed.

---

This repository demonstrates the management of IAM roles and permissions in Google Cloud, focusing on project-level roles and specific Cloud Storage access. For further details, refer to the [Google Cloud IAM documentation](https://cloud.google.com/iam/docs/overview).

