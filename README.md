# AWS CLI role for Ansible

Installs and configures the AWS CLI for conveniently interacting with AWS services such as S3.

## Requirements

Tested on CentOS 7 Server.

## Role Variables

The default variables are as follows:

    home_dir: '/root'
    aws_cli_user: 'movies'
    aws_s3_bucket: 'starwars'
    aws_output_format: 'json'
    aws_region: 'ap-southeast-2'
    aws_access_key_id: 'YOUR_ACCESS_KEY_ID'
    aws_secret_access_key: 'YOUR_SECRET_ACCESS_KEY'


## Example Playbook

    - name: Install AWS CLI
      tags: aws-cli installation
      hosts: 'servers'
      roles:
        - aws-cli

# License

This playbook is provided 'as-is' under the conditions of the BSD license. No fitness for purpose is guaranteed or implied.