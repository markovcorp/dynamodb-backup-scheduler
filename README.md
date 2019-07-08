## Dynamodb Backup Scheduler

A cloudFormation template - Since DynamoDb backup is ondemand feature - this CF template will help customer to trigger the Lambda code (Python code) in daily basis

### upload the lambda zip to s3

run `build.sh` to  create the zip file then upload to s3 bucket in the us-west-2 region which is same as cafe-prod region. then create the stack using the template file `ddb-backup-cf.json`. Fill in the parameters including s3 bucket (code bucket) and lambda zip file name etc.

### Update stack with changes

If you update the cloudformation template, you can update the stack using the modified `ddb-backup-cf.json` from the cloudformation console.
To update cloudformation tempate `ddb-backup-cf.json` you can use the nice drag and drop UI from cloudformation console!

## License

This library is licensed under the Amazon Software License.
