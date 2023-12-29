# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices on AWS.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| January 8, 2024 | Unknown | EC2 | Amazon Elastic Graphics will reach end of life on January 8, 2024. ([link](https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/elastic-graphics.html?icmpid=docs_ec2_console)) | |
| January 31, 2024 | January 31, 2023 | DeepLens |  DeepLens is retiring, including no longer having access to any DeepLens devices ([link](https://docs.aws.amazon.com/deeplens/latest/dg/deeplens-end-of-life.html)) | |
| February 1, 2024 | July 28, 2023 | EC2 - Price change |  IPv4 addresses will be charged for ([link](https://aws.amazon.com/blogs/aws/new-aws-public-ipv4-address-charge-public-ip-insights/)) | |
| March 31, 2024 | May 10, 2023 | OpsWorks |  OpsWorks for Puppet Enterprise will no longer be able to be used ([link](https://docs.aws.amazon.com/opsworks/latest/userguide/welcome_classic.html)) | |
| May 5, 2024 | May 10, 2023 | OpsWorks |  OpsWorks for Chef Automate will no longer be able to be used ([link](https://docs.aws.amazon.com/opsworks/latest/userguide/welcome_classic.html)) | |
| May 26, 2024 | May 25, 2023 | OpsWorks |  OpsWorks Stacks will no longer be able to be used ([link](https://docs.aws.amazon.com/opsworks/latest/userguide/welcome_classic.html)) | |
| July 31, 2024 | July 31, 2023 | CodeStar | AWS CodeStar is being deprecated. Existing resources will be unaffected, but you will not be able to create new resources with it. ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/84#issue-1830512424)) | |
| September 30, 2024 | November 22, 2023 | Application Cost Profiler (ACP) | AWS Application Cost Profiler (ACP) will be discontinued ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/87)) | |
| December 16, 2024 | Unknown | IoT | AWS IoT 1-Click service will be discontinued ([link](https://docs.aws.amazon.com/iot-1-click/latest/developerguide/1click-end-of-life.html)) | |
| December 31, 2024 | December 28, 2023 | Aurora Serverless | Aurora Serverless will be automatically upgraded to v2, which has some significant differences, such as not scaling down to zero. ([link](https://twitter.com/jeremy_daly/status/1740475761113604451)) | |




