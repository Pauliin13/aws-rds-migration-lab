# aws-rds-migration-lab
# AWS RDS Migration Lab

## Overview

This project demonstrates the migration of a local MariaDB database running on Amazon EC2 to Amazon RDS using AWS CLI.

## Services Used

- Amazon EC2
- Amazon RDS
- VPC
- Security Groups
- AWS CLI
- Amazon CloudWatch
- AWS Systems Manager Parameter Store

## Architecture

Application running on EC2 connected to a MariaDB database hosted on Amazon RDS inside private subnets.

## Steps Performed

1. Generated sample application data
2. Created Security Group for RDS
3. Created private subnets
4. Created DB Subnet Group
5. Created Amazon RDS MariaDB instance
6. Migrated database using mysqldump
7. Updated application database endpoint
8. Tested application connectivity
9. Monitored database metrics with CloudWatch

## Commands Used

```bash
aws rds create-db-instance
```

```bash
mysqldump --user=root --password='Re:Start!9'
```

```bash
mysql --host=<RDS-ENDPOINT>
```

## Skills Learned

- AWS CLI
- Amazon RDS
- Database migration
- Network isolation
- Security Groups
- Cloud monitoring
- Linux commands

## Result

Successfully migrated the application database from a local EC2 instance to Amazon RDS.
