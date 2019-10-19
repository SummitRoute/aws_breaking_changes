After items are a month old, they'll be moved to this page, to archive them.

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- |
| May 30, 2019 | Unknown | Lambda | Support ends for runtime .NET Core 2.0; no longer able to update ([link](https://docs.aws.amazon.com/lambda/latest/dg/runtime-support-policy.html)) | ``aws lambda list-functions --query 'Functions[?Runtime == `dotnetcore2.0`]'.FunctionName`` |
| June 1, 2019 | March 25, 2019 | Mechanical Turk | Older versions of the MTurk Requester API (2014-08-15) will stop working ([link](https://forums.aws.amazon.com/ann.jspa?annID=6686)) |  | 
| June 11, 2019 | May 14, 2019 | Lambda | Execution environment update to Amazon Linux 2018.03 ([link](https://aws.amazon.com/blogs/compute/upcoming-updates-to-the-aws-lambda-execution-environment/)) | See link |
| June 30, 2019 | Unknown | Lambda | Support ends for Node.js 6.10; no longer able to update ([link](https://docs.aws.amazon.com/lambda/latest/dg/runtime-support-policy.html)) | ``aws lambda list-functions --query 'Functions[?Runtime == `nodejs6.10`]'.FunctionName`` |
| July 22, 2019 | May 21, 2019 | EKS | Kubernetes 1.10 force updated to 1.11 ([docs](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html) and [blog](https://aws.amazon.com/blogs/compute/updates-to-amazon-eks-version-lifecycle/)) |  |
| July 31, 2019 | Unknown | Lambda | Support ends for runtimes .NET Core 1.0 and 1.1; no longer able to update ([link](https://docs.aws.amazon.com/lambda/latest/dg/runtime-support-policy.html)) | ``aws lambda list-functions --query 'Functions[?Runtime == `dotnetcore1.0`]'.FunctionName`` |
| October 16, 2019 | Unknown | Elastic Beanstalk | Windows Server 2008 R2 retired ([link](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/platforms-support-policy.html)) |  |
