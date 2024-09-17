# AWS S3 Bucket Module

This module creates an AWS S3 bucket with optional tagging.

## Usage

```hcl
module "s3_bucket" {
  source      = "git::ssh://git@your-private-repo.com/terraform-modules/aws-s3-bucket.git"
  bucket_name = "my-bucket"
  tags = {
    Environment = "Dev"
    Team        = "DevOps"
  }
}

Testing
