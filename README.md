# spring-cloud-aws-examples

### Steps
- Create AWS bucket
```bash
$ aws s3api create-bucket --bucket spring-cloud-bucket --create-bucket-configuration LocationConstraint=ap-southeast-2

{
    "Location": "http://spring-cloud-bucket.s3.amazonaws.com/"
}
```

