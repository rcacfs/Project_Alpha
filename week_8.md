# Project_Alpha
## Week 8
### Backup

#### Task 1: IAM Role & Policy
- Create IAM roles and policies that allow the AWS Backup service to access the resources to be backed up.
- Assign the IAM role to the AWS Backup service.

#### Task 2: Backup Plan
- Create a backup plan that defines the backup frequency, retention period, lifecycle rules, and backup vault for the backups.
- Add the AWS instances' EBS volumes and RDS Postgresql as backup selections to the backup plan.
- Monitor the backup jobs and restore jobs using the AWS Backup console or API.

#### Task 3: Backup Automation - Terraform
- Define IAM roles and policies to reference AWS Backup resources in your Terraform template: Leverage the reference material below.
- Define a backup vault, the management dashboard of your backups.
- Define a backup plan that defines the backup frequency, retention period, lifecycle rules, and a selection of resources to be backed up.
- Verify your backups on the AWS console under Backup Vaults

## References
https://shadabambat1.medium.com/automatically-backup-your-ec2-instances-using-aws-backups-terraform-c06d15e2a9c2
