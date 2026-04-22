# Client CFN IAM Role

Welcome to the Braid Access Repository. You’ve just created an AWS account, and now it’s time to grant us access so we can manage your account and deploy the infrastructure, including the necessary software, into your AWS environment. Since security is very important to us, we request access to your account through an IAM role that we will assume. This role allows us to efficiently and securely access your account to perform all the required tasks.

The deployment process is straightforward, and this guide will walk you through it step by step.

## Preparation Steps

1. Open a new tab and log into your new AWS account using the **root user** (the email and password you used to create the account).  
1. Verify that you have selected the correct region: **us-east-1 (Virginia)**.  
1. Once you've confirmed the above, click the following link to open the AWS CloudFormation Console with a prefilled template: **[Click here to start](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=braid-access&templateURL=https://braid-438465148503-us-east-1-cdn.s3.us-east-1.amazonaws.com/cfn/client_cfn_iam_role.json)**.  

## Deploying the Template

1. In the newly opened tab, click the orange `Next` button.  
1. On the next page, simply click the orange `Next` button again.  
1. On the next page, click the orange `Next` button again.  
1. Scroll down until you see the **Capabilities and transforms** section. Check all the boxes, then click the orange `Submit` button.  
1. You will be redirected to a new page where you can monitor the deployment process.  

## Final Steps

1. Once the deployment status shows **all green**, click the **Outputs** tab.  
1. In the Outputs tab, locate the table and send us the value listed under the key `AccountId` from the Outputs tab of the CloudFormation stack.  

## Congratulations

You’ve successfully completed the setup! From this point onward, we’ll handle the rest of the process. Thank you for your cooperation.

## About the Role

The role created by this CloudFormation template grants us the necessary access to manage your AWS account efficiently and securely. While this role has administrator-level permissions, we have implemented safeguards to prevent critical actions, such as creating new users or disabling logs, from being performed unintentionally.

These safeguards are in place to protect your account and make sure everything stays secure while we manage it.

By using this role, we can handle everything necessary to set up and maintain your account without creating any potential risks.
