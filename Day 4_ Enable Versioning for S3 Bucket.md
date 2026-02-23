# Day 4: Enable Versioning for S3 Bucket

Data protection and recovery are fundamental aspects of data management. It's essential to have systems in place to ensure that data can be recovered in case of accidental deletion or corruption. The DevOps team has received a requirement for implementing such measures for one of the S3 buckets they are managing.

The s3 bucket name is xfusion-s3-13870, enable versioning for this bucket.

✅ Method 1: Using the AWS Management Console

1. Sign in to the AWS Management Console and open the Amazon S3 console.
<img width="1376" height="462" alt="Image" src="https://github.com/user-attachments/assets/50256bbf-a599-40e8-bcb3-ac03007b62b0" />

3. Select the desired bucket from the Buckets list.
4. Navigate to the Properties tab.

<img width="1909" height="618" alt="Screenshot 2026-02-22 105025" src="https://github.com/user-attachments/assets/d7073032-1c08-4a88-aba9-b17be586b791" />


6. Scroll down to find the Bucket Versioning section and select Edit.
<img width="1912" height="679" alt="Screenshot 2026-02-22 105119" src="https://github.com/user-attachments/assets/291fafd6-b11e-4f27-885b-79f8436e02a5" />

7. Choose Enable.
8. Select Save changes to apply the setting

✅ Method 2: Using the AWS CLI

Ensure you have the AWS CLI installed and configured with appropriate permissions. Then, run the following command, replacing bucket-name with your actual bucket name:

```
aws s3api put-bucket-versioning --bucket bucket-name --versioning-configuration Status=Enabled
```
