# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| March 31, 2021 | March 31, 2020 | FIPS | TLS 1.2 to become the minimum for all AWS FIPS endpoints [link](https://aws.amazon.com/blogs/security/tls-1-2-to-become-the-minimum-for-all-aws-fips-endpoints/) | |
| June 1, 2021 | October 20, 2020 | Lambda | Python 2.7 run-time being deprecated ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/34)) | |
| July 15, 2021 | January 19, 2021 | SDK | End of support for Python 2.7 for the SDK and CLI ([link](https://aws.amazon.com/blogs/developer/announcing-end-of-support-for-python-2-7-in-aws-sdk-for-python-and-aws-cli-v1/)) | |
| August 1, 2021 | August 1, 2020 | Config | Indirect relationship recording removed from EC2s ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/42)) | |
| October 30, 2021 | July 28, 2020 | EC2 | EC2-Classic is being retired ([link](https://aws.amazon.com/blogs/aws/ec2-classic-is-retiring-heres-how-to-prepare/)) | |
