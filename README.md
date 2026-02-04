# Host a Website on Amazon S3 ☁️

## 📌 Project Overview
This project demonstrates how to host a **static website** using **Amazon S3**. The objective of this project was to understand how Amazon S3 stores and retrieves data and how it can be used to host a publicly accessible website.

---

## 🛠️ AWS Service Used
- **Amazon S3 (Simple Storage Service)**

---

## 🔹 Key Concepts Learned
- Creating and configuring an S3 bucket  
- Understanding that S3 bucket names are globally unique  
- Uploading files to S3  
- Enabling Static Website Hosting  
- Understanding and configuring **ACLs (Access Control Lists)**  
- Troubleshooting a **403 Forbidden error**

---

## 🚀 Step-by-Step Procedure

### **Step 1: Create an S3 Bucket**
1. Logged into the AWS Management Console.
2. Navigated to **Amazon S3**.
3. Clicked on **Create Bucket**.
4. Chose **Asia Pacific (Mumbai)** as the region since it is the closest location.
5. Gave a unique bucket name (S3 bucket names must be globally unique).
6. Created the bucket successfully.

---

### **Step 2: Upload Website Files to S3**
1. Opened the created S3 bucket.
2. Clicked on **Upload**.
3. Uploaded:
   - `index.html` (main webpage file)
   - A folder containing 44 supporting files (images and assets).
4. Verified that all files were successfully uploaded.

---

### **Step 3: Enable Static Website Hosting**
1. Opened the **Properties** tab of the S3 bucket.
2. Scrolled to **Static Website Hosting** section.
3. Selected **Enable**.
4. Set:
   - Index document: `index.html`
5. Saved the changes.

---

### **Step 4: Access Bucket Endpoint**
1. After enabling static hosting, S3 generated a **Bucket Endpoint URL**.
2. Opened the endpoint URL in a browser.
3. Received a **403 Forbidden error**.

---

### **Step 5: Fix 403 Forbidden Error (Configure ACLs)**
1. Went to the **Permissions** tab of the S3 bucket.
2. Enabled **Access Control Lists (ACLs)**.
3. Changed the permissions of:
   - `index.html`
   - The images/assets folder  
   to **Public Read Access**.
4. Reloaded the website endpoint.

---

## ✅ Final Result
The website was successfully hosted and became publicly accessible using Amazon S3.

---

## 📂 Project Files
