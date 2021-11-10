# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| August 30, 2021 | July 30, 2021 | Lambda | No longer retrying errors when Lambda concurrency is zero ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/48)) | |
| September 8, 2021 | September 4, 2021 | ElasticSearch/IAM | IAM privilege names for ElasticSearch changed ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/52)) | |
| September 15, 2021 | August 1, 2020 | Config | Indirect relationship recording removed from EC2s ([link](https://docs.aws.amazon.com/config/latest/developerguide/faq.html#faq)) | |
| October 20, 2021 | September 27, 2021 | CloudWatch Events/Lambda | Lambda API names in CloudTrail/CloudWatch Events will no longer include the version in the API name ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/53)) | |
| On or before October 26th | Unknown | Event Bridge/Step Functions | Event Bridge rules can no longer trigger Step Functions state machine executions on an `Step Functions Execution Status Change` event from the same state machine | | 
| November 22, 2021 | September 2, 2021 | Cloudtrail | Global service events only available in Lookup in us-east-1 ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/51)) | |
| December 1, 2021 | August 31, 2021 | Athena | Query syntax changes ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/49)) | |
| April 29, 2022 | May 14, 2021 | S3 | S3 BitTorrent support to be turned off for customers who have it enabled in their account ([link](https://github.com/awsdocs/amazon-s3-userguide/commit/0d1759880ccb1818ab0f14129ba1321c519d2ac1#diff-72be9d82d9be9bda6a297a4fbd11aca66ecde97e4f90de6f86bdf95c5f6b72c0R3)) | |
| August 15, 2022 | July 28, 2021 | EC2 | EC2 classic retiring ([link](https://aws.amazon.com/blogs/aws/ec2-classic-is-retiring-heres-how-to-prepare/)) | |
| July 31, 2022 | July 29, 2021 | Console | IE 11 support ending for console ([link](https://aws.amazon.com/blogs/aws/heads-up-aws-support-for-internet-explorer-11-is-ending/)) | |
| December 31, 2022 | Unknown | EC2 | Spot blocks (defined duration) are no longer supported ([docs](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-requests.html#fixed-duration-spot-instances), [api](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_RequestSpotInstances.html)) | |
