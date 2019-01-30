# spring-cloud-aws-examples

### Steps
- Create AWS bucket
```bash
$ aws s3api create-bucket --bucket spring-cloud-bucket --create-bucket-configuration LocationConstraint=ap-southeast-2

{
    "Location": "http://spring-cloud-bucket.s3.amazonaws.com/"
}
```
- Run the app:
```bash
./mvnw spring-boot:run -Dspring-boot.run.arguments=--aws.credentials.accessKey=<your_access_key>,--aws.credentials.secretKey=<your_secret_key>
```
- Download it:
```bash
$ http://localhost:8080/download/spring-cloud-bucket/example/beer.jpg
```
