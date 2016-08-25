aws-ssh
=======

Convenience bash function for SSH on EC2.

Usage
=====

```shell
aws-ssh [-h] [[user@]host] [--profile aws_profile] [--region aws_region]
```

Returns a list of EC2 machines with a `Name` tag that fuzzy matches the `host`
argument, then initiates an SSH session with that machine.

```
$ aws-ssh drew --region us-west-2
1) drew-efs-loader  i-0de1f14d8dccf1c2c  10.10.0.5  None
#? 1
Connecting to host 10.10.0.5 as ..
```
