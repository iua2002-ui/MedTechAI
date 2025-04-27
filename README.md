# MedTech AI Secure S3 Bucket

Terraform module to deploy a HIPAA-compliant S3 bucket for AI training data.

## Usage

```terraform
module "medtech_s3" {
  source    = "github.com/your-iua2002/medtech-ai-s3-terraform//modules/s3"
  bucket_name = "medtech-ai-data-123"
  region      = "us-east-1"
}
```

## Requirements
- Terraform >= 1.6
- AWS provider >= 5.0

## Security Controls
- Server-side encryption (SSE-S3/KMS)
- Versioning enabled
- Public access blocked
