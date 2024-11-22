# Client CFN IAM Role

Welcome to the Braid Access Repository. You’ve just created an AWS account, and now it’s time to grant us access so we can manage your account and deploy the infrastructure, including the necessary software, into your AWS environment. Since security is very important to us, we request access to your account through an IAM role that we will assume. This role allows us to efficiently and securely access your account to perform all the required tasks.

The deployment process is straightforward, and this guide will walk you through it step by step.

## Preparation Steps

1. Open a new tab and ensure you are logged into your new AWS account.  
1. Verify that you have selected the correct region: **us-east-1 (Virginia)**.  
1. Once you’ve confirmed the above, click the following link to open the AWS CloudFormation Console with a prefilled template: **[Click here to start](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=braid-access&templateURL=https://braid-438465148503-us-east-1-cdn.s3.us-east-1.amazonaws.com/cfn/client_cfn_iam_role.json)**.  

## Deploying the Template

1. In the newly opened tab, click the orange `Next` button.  
1. On the next page, simply click the orange `Next` button again.  
1. Scroll down on the following page until you see the **Capabilities and transforms** section. Check all the boxes, then click the orange `Next` button.  
1. Scroll down on the next page and click the orange `Submit` button.  
1. You will be redirected to a new page where you can monitor the deployment process.  

## Final Steps

1. Once the deployment status shows **all green**, click the **Outputs** tab.  
1. In the Outputs tab, locate the table and send us the value listed under the key `AccountId`.  

## Congratulations

You’ve successfully completed the setup! From this point onward, we’ll handle the rest of the process. Thank you for your cooperation.

## About the Role

The role created by this CloudFormation template gives us the access needed to manage your AWS account efficiently and securely. This role has administrator-level access, but we’ve also added extra safety measures to ensure that no critical or sensitive actions, like creating new users or disabling logs, can happen by mistake.

These safeguards are in place to protect your account and make sure everything stays secure while we manage it.

By using this role, we can handle everything necessary to set up and maintain your account without creating any potential risks.
