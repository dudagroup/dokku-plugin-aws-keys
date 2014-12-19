dokku-plugin-aws-keys
=====================

Plugin to assign was keys to a docker app, so that it's instantly available in the environment.

EC2 Policy
```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": [
                "iam:GetGroup",
                "iam:CreateGroup",
                "iam:CreateUser",
                "iam:AddUserToGroup",
                "iam:DeleteAccessKey",
                "iam:CreateAccessKey"
            ],
            "Resource": "*"
        }
    ]
}
```
