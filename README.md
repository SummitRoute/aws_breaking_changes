# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| April 30, 2022 | Feb 3, 2022 | IAM Lambda | IAM policy evaluation being changed for how Lambda ARNs are referrenced ([link](https://forum.serverless.com/t/lambda-security-notification-from-aws-involving-iam-policies-need-help-determining-action-for-serverless-framework/16660)) | |
| May 18, 2022 | Dec 30, 2021 | RDS, Aurora (GovCloud) | Database connections that use TLS certificate validation must use the new `rds-ca-rsa4096-g1` CA certificate or connections will fail. Starting March 21, all new databases will use the new CA certificate; starting May 18, all databases will starting having certificate rotations scheduled during their maintenance window. |  |
| August 15, 2022 | July 28, 2021 | EC2 | EC2 classic retiring ([link](https://aws.amazon.com/blogs/aws/ec2-classic-is-retiring-heres-how-to-prepare/)) | |
| August 17, 2022 | April 15, 2022 | Lambda | Python 3.6 run-time deprecated ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/61))
| July 31, 2022 | July 29, 2021 | Console | IE 11 support ending for console ([link](https://aws.amazon.com/blogs/aws/heads-up-aws-support-for-internet-explorer-11-is-ending/)) | |
| December 31, 2022 | Unknown | EC2 | Spot blocks (defined duration) are no longer supported ([docs](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-requests.html#fixed-duration-spot-instances), [api](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_RequestSpotInstances.html)) | |
