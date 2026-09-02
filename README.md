# Workspace Image Building Process
1. Create a Directory
2. Go to AWS Workspace Register your directory
3. Create a Image User and Password This user will have temporary workspace
4. Now Create a workspace for this user.
5. Create a preassign url for the package s3 bucket.- Using AWS Console
   ```
   curl -fL '<SSM-PRESIGNED-URL>' \
  -o /tmp/amazon-ssm-agent.rpm
   sudo rpm -Uvh /tmp/amazon-ssm-agent.rpm
   sudo systemctl enable --now amazon-ssm-agent
   systemctl status amazon-ssm-agent
```
7. Now install aws cli and ssm manager.
8. Once up and running verify aws cli and ssm is up and running and then create image bundle.
9. Copy the bundle ID and go to Parameter Store and Update the Bundle ID.

https://docs.aws.amazon.com/workspaces/latest/adminguide/cloudformation-templates.html


   
