Q2. Write an ansible playbook to create and instance that can store items in S3.

Manually created S3 bucket for test purposes.

Get access key and secret access key of aws user with sufficient rights to spin up an ec2 instance.

Then set following environmental variables
```
export AWS_ACCESS_KEY=<access key>
export AWS_SECRET_ACCESS_KEY=<secret access key>
```

Then run command
```
ansible-playbook -i ./hosts ec2.yml
'''

Note: 1st time it fails because `instance profile` has not been created in time to be attached to ec2 instance.
