# Day 20: Create IAM Role for EC2 with Policy Attachment

Create an IAM role as below:

- IAM role name must be `iamrole_ammar`.
- Entity type must be `AWS Service` and use case must be `EC2`.
- Attach a policy named `iampolicy_ammar`.

## To create IAM role for custom policy.

1. Go to IAM Dashboard and choose `Roles` from navigation pane.

   <img width="263" height="472" alt="image" src="https://github.com/user-attachments/assets/e89eecb4-7b2f-4081-a147-b463f8806425" />

2. Click `Create role` and select `AWS service` under `Trusted Entity Type`

   <img width="1325" height="435" alt="image" src="https://github.com/user-attachments/assets/7d4e67ff-cd1c-493e-9adc-2076c482a23c" />

3. Under `Use case`, select `EC2` and click `Next` to proced on step 2.

   <img width="1015" height="364" alt="image" src="https://github.com/user-attachments/assets/423e44d8-bad9-4c2b-b783-6e4d14887f05" />

4. On step 2, in the `Permission policy` tab, search for the custom policy and select it.

   
   <img width="1906" height="556" alt="image" src="https://github.com/user-attachments/assets/9ba53370-a881-4e3f-b492-1bab301b15f9" />


5. On step 3, enter preferred role name and click on `Create role`.

   
   <img width="1905" height="481" alt="image" src="https://github.com/user-attachments/assets/313c7bbb-e0fa-4d03-ba45-20ca57bdf640" />

   <img width="1872" height="755" alt="image" src="https://github.com/user-attachments/assets/3d37252e-901b-4fae-9371-e441ed4f1ef7" />




