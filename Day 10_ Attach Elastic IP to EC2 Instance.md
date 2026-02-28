# Day 10: Attach Elastic IP to EC2 Instance

There is an instance named devops-ec2 and an elastic-ip named devops-ec2-eip in us-east-1 region. Attach the devops-ec2-eip elastic-ip to the devops-ec2 instance.

AWS Documentation to be folllowed: [Associate an Elastic IP address](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/working-with-eips.html#using-instance-addressing-eips-associating)

To associate an Elastic IP address with an instance

1. Open the Amazon EC2 console at https://console.aws.amazon.com/ec2/

3. In the navigation pane, choose **Elastic IPs**.
  
6. Select the Elastic IP address to associate and choose **Actions, Associate Elastic IP address**.

   <img width="1920" height="908" alt="image" src="https://github.com/user-attachments/assets/d9ec7b02-d69c-4a5f-a9a4-9def0dc98dd7" />


8. For **Resource type**, choose **Instance**.
  
   <img width="1913" height="903" alt="image" src="https://github.com/user-attachments/assets/5844413e-9bb4-4b81-9187-409cc17d3956" />

10. For instance, choose the instance with which to associate the Elastic IP address. You can also enter text to search for a specific instance.

11. (Optional) For **Private IP** address, specify a private IP address with which to associate the Elastic IP address.

12. Choose **Associate**.
    <img width="1919" height="910" alt="image" src="https://github.com/user-attachments/assets/5bb9ee73-bf9b-4358-a67f-2efc82fc3385" />
