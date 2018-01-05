Get access key and secret access key of aws user with sufficient rights to spin up an ec2 instance.

Then set following environmental variables
```
export AWS_ACCESS_KEY=<access key>
export AWS_SECRET_ACCESS_KEY=<secret access key>
```

I could not find a way to create an instance profile; for now created it manually.

Then run command
```
ansible-playbook -i ./hosts ec2.yml
```
