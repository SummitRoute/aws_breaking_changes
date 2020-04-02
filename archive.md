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
| November 4, 2019 | Unknown | EKS | No longer able to use Kubernetes 1.11 and forced to upgrade to 1.12 ([link](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html#version-deprecation)) |  |
| January 6, 2020 | October 18, 2019 | Lambda | Support ends for Node.js 8.10, no longer able to create functions. Feb 3, no longer able to update. ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/27)) |  |
| January 15, 2020 | August 5, 2019 | RDS | PostgreSQL 9.4 instances will be force upgraded to PostgreSQL 11 ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/30)) |  |
| February 5, 2020 | January 7, 2020 | RDS, Aurora, DocumentDB | Database connections that use TLS certificate validation must use a new CA, or connections will fail.  Any of these databases that are restarted after Feb 5 will use the new CA. All databases (whether or not they are restarted) will enforce the new CA after March 5, 2020, ([link](https://aws.amazon.com/blogs/aws/urgent-important-rotate-your-amazon-rds-aurora-and-documentdb-certificates/))|  |
| March 1, 2020 | Unknown | Elastic Beanstalk | Apache HTTP Server 2.2, Nginx 1.12.2, GlassFish 4.x, Go 1.3–1.10, Java 6, Node.js 4.x–8.x, PHP 5.4–5.6, PHP 7.0–7.1, Python 2.6, 2.7, 3.4, Ruby 1.9.3, Ruby 2.0–2.3, Tomcat 6, Tomcat 8 ([link]
