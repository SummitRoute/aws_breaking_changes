# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| November 14, 2022 | August 14, 2022? | Lambda | Node.js 12 run-time end-of-life ([link](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html#runtime-support-policy)) | |
| December 31, 2022 | Unknown | EC2 | Spot blocks (defined duration) are no longer supported ([docs](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-requests.html#fixed-duration-spot-instances), [api](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_RequestSpotInstances.html)) | |
| January 20, 2023 | August 14, 2022 | Lambda | .NET Core 3.1 run-time end-of-life ([link](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html#runtime-support-policy)) | |
| February 21, 2023 | May 18, 2022 | Amazon Sumerian |  Amazon Sumerian retiring ([link](https://aws.amazon.com/blogs/aws/amazon-sumerian-now-generally-available/)) | |
| June 28, 2023 | June 28, 2022 | TLS | APIs will no longer support TLS versions 1.0 and 1.1 ([link](https://aws.amazon.com/blogs/security/tls-1-2-required-for-aws-endpoints/)) | |
| September 1, 2023 | September 1, 2022 | Amazon WAM |  Amazon WorkSpaces Application Manager retiring ([link](https://aws.amazon.com/blogs/desktop-and-application-streaming/amazon-workspaces-application-manager-amazon-wam-is-retiring/)) | |


