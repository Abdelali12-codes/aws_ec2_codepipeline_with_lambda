# aws_ec2_codepipeline_with_lambda

## lambda policy to invoke codepipeline

```
{
  "Version": "2012-10-17", 
  "Statement": [
    {
      "Action": [ 
        "logs:*"
      ],
      "Effect": "Allow", 
      "Resource": "arn:aws:logs:*:*:*"
    },
    {
      "Action": [
        "codepipeline:PutJobSuccessResult",
        "codepipeline:PutJobFailureResult"
        ],
        "Effect": "Allow",
        "Resource": "*"
     }
  ]
} 

```
