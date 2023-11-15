
## Week 5
### Databases (RDS Postgresql) 

#### Task 1: RDS Instance Creation
- Create an Amazon RDS instance for PostgreSQL.
- Specify the instance class, storage size, and other relevant configurations.
- Configure the database identifier, master username, and password.

#### Task 2: VPC and Security Group Configuration
- Set up the Virtual Private Cloud (VPC) to host the RDS instance.
- Configure security groups to control inbound and outbound traffic to the RDS instance.
- Ensure proper network ACLs and route tables are in place for secure communication.

#### Task 3: Database Schema and Users
- Develop scripts or configurations for creating the necessary database schema and tables.
- Set up PostgreSQL users with appropriate permissions.
- Include any initial data seeding or configuration required for the database.

#### Task 4: Backups and High Availability
- Configure automated backups for the RDS instance.
- Implement a strategy for database snapshots and retention.
- Explore and set up Multi-AZ deployment for high availability if needed.

#### Task 5: Monitoring and Logging
- Set up monitoring for the RDS instance using Amazon CloudWatch.
- Configure relevant alarms based on performance metrics.
- Enable and configure database logs for auditing and troubleshooting.

### S3 (Storage for static media files)

#### Task 1: S3 Bucket Creation
- Create an Amazon S3 bucket to store the static media files.
- Choose a unique and meaningful bucket name.
- Configure the region for the bucket.

#### Task 2: Bucket Policies and Permissions
- Define and apply a bucket policy to control access to the S3 bucket.
- Set up appropriate permissions for IAM users, roles, or groups that need access to the bucket.
- Consider using AWS Identity and Access Management (IAM) roles for secure access.

#### Task 3: Versioning and Logging
- Enable versioning for the S3 bucket to maintain different versions of files.
- Configure logging to capture detailed information about bucket access and changes.
- Specify the target bucket for logs to facilitate auditing and analysis.

#### Task 4: Configure S3 bucket for media storage
- Modify the application to handle file uploads and save them to S3
