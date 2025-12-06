# Automation Command to create an s3 bucket
aws s3api create-bucket \
  --bucket clam-bucket20009 \
  --region us-east-2 \
  --create-bucket-configuration LocationConstraint=us-east-2

# Automation Command to delete an s3 bucket
aws s3api delete-bucket \
  --bucket clam-bucket20009 \
  --region us-east-2

# Aws automation 2 using aws cli 

### command to create iam user in aws
aws iam create-user --user-name <username>

### command to list out iam users
aws iam list-users

### command to delete iam users in aws using the cli
aws iam delete-user --user-name <username>

### to delete keypair using cli
 aws ec2 delete-key-pair --key-name <keyname>

 ### to how how many key pairs you have 
 aws ec2 describe-key-pairs

 ### to describe an ec2 instance using cli.     
aws ec2 describe-instances --instance-ids i-04c945ceff455a7e1