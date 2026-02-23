# Day 5: Create GP3 Volume

For this task, Create a volume with the following requirements:

Name of the volume should be `xfusion-volume`.

- Volume type must be gp3.

- Volume size must be 2 GiB.


1. Open the Amazon EC2 console at https://console.aws.amazon.com/ec2/

   <img width="1918" height="907" alt="image" src="https://github.com/user-attachments/assets/b8628403-c64b-41f2-8a6f-1c3d3a7c318f" />


3. In the navigation pane, choose Volumes and then choose `Create volume`.

  <img width="1916" height="536" alt="image" src="https://github.com/user-attachments/assets/ac9d4d15-475c-4c87-9f91-60daec6d89ff" />

5. (Outpost customers only) For Outpost ARN, enter the ARN of the AWS Outpost on which to create the volume.

6. For Volume type, choose the type of volume to create. For more information about the available volume types, see Amazon EBS volume types.

7. For Size, enter the size of the volume, in GiB. For more information, see Amazon EBS volume constraints.

8. (For io1, io2, and gp3 only) For IOPS, enter the maximum number of input/output operations per second (IOPS) that the volume should provide.

9. (For gp3 only) For Throughput, enter the throughput that the volume should provide, in MiB/s.

10. For Availability Zone, choose the Availability Zone in which to create the volume.

11. Choose `Create volume`.
    <img width="1107" height="768" alt="image" src="https://github.com/user-attachments/assets/64514ec1-231c-4fb3-8c74-f8991ec54937" />

  
13. After creating the volume, rename it with `xfusion-volume` [For the task only]
    <img width="1919" height="331" alt="image" src="https://github.com/user-attachments/assets/2ec2848f-307e-4a3b-9afc-93f2db54aa91" />


15. To use the volume, wait for it to reach the available state and then attach it to an Amazon EC2 instance in the same Availability Zone.
    <img width="1659" height="241" alt="image" src="https://github.com/user-attachments/assets/3131614f-b123-496c-bbda-1430672bd317" />

