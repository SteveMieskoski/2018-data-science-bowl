# Command line examples

Launch an instance
```bash 
aws ec2 request-spot-instances --cli-input-json file://launch-p2-spot.json
```

Get the status of running instances
```bash
aws ec2 describe-instance-status
```

Get the publicDnsName of an instance using it's instanceID
```bash
aws ec2 describe-instances --instance-ids <yourinstanceid> --query 'Reservations[*].Instances[*].[PublicDnsName]'
```
