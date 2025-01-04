# aws_resource_tracker
# This scripy will report the aws resourse usage.
##########################################
# Author : Harshad
#  Date : 27/12/2024
#
#  Version : v1
#
#  This scripy will report the aws resourse usage
#
set -x

#AWS S3
#AWS EC2
#AWS Lambda
#AWS IAM Users

# List S3 buckets
echo "Print list of S3 buckets"
aws s3 ls resourceTracker

# list EC2 Instances
echo "Print list of EC2 instances"
aws ec2 describe-instances resourceTracker

# list lambda
echo "Print list of lambda"
aws lambda list-functions resourceTracker

# list IAM users
echo "Print list of IAM users"
aws iam list-users resourceTracker
