# Day 18: Create Read-Only IAM Policy for EC2 Console Access

Create an IAM policy named `iampolicy_ammar` in `us-east-1` region, it must allow read-only access to the EC2 console, i.e this policy must allow users to view all instances, AMIs, and snapshots in the Amazon EC2 console.

AWS DOcs to be followed: [Create IAM policies (console)](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_create-console.html#access_policies_create-json-editor)

## To use the JSON policy editor to create a policy

1. Sign in to the `AWS Management Console` and open the IAM console at [https://console.aws.amazon.com/iam/](https://console.aws.amazon.com/iam/)

   <img width="987" height="446" alt="image" src="https://github.com/user-attachments/assets/f64ff977-879b-4676-8b34-9b3257915b50" />

2. In the navigation pane on the left, choose `Policies`.

   <img width="263" height="466" alt="image" src="https://github.com/user-attachments/assets/3d69cac5-ce9b-4cd9-bea3-25bab85bda2a" />

3. Choose `Create policy`.

   <img width="1054" height="141" alt="image" src="https://github.com/user-attachments/assets/6793a244-acef-4e73-9153-968d0b9e35fc" />

4. In the `Policy editor` section, choose the `JSON` option and add below content.
```
   {
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": [
                "ec2:Describe*",
                "ec2:Get*",
                "ec2:List*"
                
            ],
            "Resource": "*"
        }
      
    ]
}
```
   <img width="1884" height="891" alt="image" src="https://github.com/user-attachments/assets/085ac14c-41f4-4ea9-b34e-318acf772dbc" />

   <img width="1328" height="337" alt="image" src="https://github.com/user-attachments/assets/84dfb468-d5ee-4792-b729-519b250b4c9a" />

5. On the `Review and create` page, type a `Policy Name` and a `Description (optional)` for the policy that you are creating. Review the Permissions defined in this policy to make sure that you have granted the intended permissions.

    
    <img width="1897" height="862" alt="image" src="https://github.com/user-attachments/assets/02c2391f-5d3c-482c-a268-a06d692bc0e8" />


6. Choose Create policy to save your new policy.

    

