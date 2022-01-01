# github-runner-ecs
CloudFormation stack for quickly deploying a Github Actions runner in Elastic Container Service in AWS

## Parameters
| Parameter Name | Description |
|----------------|-------------|
| AmiId | You must specify an ECS-optimised Amazon Linux AMI ID for this parameter |
| InstanceType | EC2 Instance type - see [https://aws.amazon.com/ec2/instance-types]() for the list |
| VpcId | VPC to deploy the EC2 instance into - this can be the default VPC for the region |
| SubnetId | Subnet inside the provided VPC to deploy the EC2 instance into |
| ClusterName | A name to identity the ECS cluster |
| LogRetentionInDays | The logs for the Github Runner container are stored in CloudWatch and this parameter controls retention |
| GithubActionRunnerName | The display name for the runner in Github |
| GithubActionsRunnerRepoUrl | The repository or organisation URL of the Github runner (provided on the runner setup page) |
| GithubActionsRunnerToken | The token for the runner (provided on the runner setup page) |

## AWS Components
| Component | Description |
|-----------|-------------|

