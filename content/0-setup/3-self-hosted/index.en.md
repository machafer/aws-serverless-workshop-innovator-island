---
title: Self-hosted
weight: 12
---

### Create an AWS account

::alert[Proceed with creating an IAM user if you already have an account, otherwise create a new AWS account first.]{type="warning"}

If you _don't_ have a root **AWS account** yet, [click](https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/) here to create a AWS account.


---
### Create an IAM user

If you already **have an AWS account** or **create an AWS account**, create an **IAM user** that has access to AWS account. Log in to the AWS account, you can create a IAM user using IAM console. Create an IAM user with Administrator role as below the step. If you already have an IAM user with administrator role, skip the next task.
1. From the [Log in Page](https://console.aws.amazon.com/), log in with AWS root account email address and password then go to [IAM Console](https://console.aws.amazon.com/iam/home#/home).
2. From the left sidebar of the IAM Console, click **Users** and then click **Add user**
3. Enter **User name** as `Administrator`.
4. Tick **AWS Management Console access** check box from Access type and then choose **Custom password** and enter the password
5. Click **Next: Permissions**
![IAM User Create](/static/images/preparation_guide/iam-user-01.png)
6. Choose **Attach existing policies directly**, tick **AdministratorAccess** option and then click **Next: Tags**
![IAM User Create](/static/images/preparation_guide/iam-user-02.png)
1. Click **Next: Review** from Add tags(optional) section.
2. Review AdministratorAccess, AWS managed policy, is added to Administrator user and then click **Create user**
3. After creating the user, copy the **login URL**. The format of the URL is as below.
`https://<your_aws_account_id>.signin.aws.amazon.com/console`
::alert[Replace <your_aws_account_id> with the unique ID of your own AWS account. We don't recommend to proceed the lab with root user. Please login with the Administrator user and proceed the lab.]{type="warning"}
![IAM User Create](/static/images/preparation_guide/iam-user-03.png)
10. Log out from the root user and then **log in to the Administrator user you just created** using the URL you copied above.