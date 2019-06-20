# cloudformation-s3-bucket-creation
Create S3 Bucket by using CloudFormation templates

  * To run this cloudformation template you can use via GUI/CLI.
  * To run this via CLI you need to install AWS CLI.
  * Follow the below links to install the AWS CLI.
  
## Installing the AWS CLI
https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html


## Install the AWS CLI on Linux
https://docs.aws.amazon.com/cli/latest/userguide/install-linux.html


## Install the AWS CLI on Windows
https://docs.aws.amazon.com/cli/latest/userguide/install-windows.html


## Install the AWS CLI on macOS
https://docs.aws.amazon.com/cli/latest/userguide/install-macos.html


## Install the AWS CLI in a Virtual Environment
https://docs.aws.amazon.com/cli/latest/userguide/install-virtualenv.html


## Install the AWS CLI Using the Bundled Installer (Linux, macOS, or Unix)
https://docs.aws.amazon.com/cli/latest/userguide/install-bundle.html

## Configure the AWS CLI
https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html

## Validate CloudFormation Json Templates
```
aws cloudformation validate-template --template-body file://create_s3_bucket.json
```

## Create Stack In CloudFormation
  * The region you have configured in the AWS CLI, It will create the S3 bucket in the same region.
```
aws cloudformation create-stack --stack-name s3bucketcreation --template-body file://create_s3_bucket.json
```

## Delete Stack
```
aws cloudformation delete-stack --stack-name iam-stack
```

## License
MIT License

Copyright (c) [2019] [ABHIJIT SHARMA]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
