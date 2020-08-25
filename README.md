# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| September 21, 2020 | August 25, 2020 | Pinpoint | Price increase of sending SMS messages to India from $0.00223 to $0.00303 per message. ([link](https://aws.amazon.com/about-aws/whats-new/2020/08/price-change-notice-for-customers-using-amazon-pinpoint-to-send-sms-messages-to-india/)) resulting from government mandata ([link](https://economictimes.indiatimes.com/industry/telecom/telecom-news/telemarketers-tear-up-as-telcos-hike-bulk-sms-fees-by-25-30/articleshow/77206891.cms?from=mdr)) | |
| September 30, 2020 | April 30, 2019 | S3 | Buckets created after September 30, 2020 must be accessed in the form \<bucketname\>.s3.amazonaws.com, not s3.amazonaws.com/\<bucketname\>/ ([link](https://aws.amazon.com/blogs/aws/amazon-s3-path-deprecation-plan-the-rest-of-the-story/)) | See link |
| October 1, 2020 | June 1, 2020 | SES | Signature must be v4. Announced privately via emails, [example](https://wordpress.org/support/topic/amazon-ses-api-signature-version-4-2/) | | 
| December 31, 2020 | December 10, 2019 | Lambda | Python 2.7 run-time being deprecated ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/34)) | |
| December 31, 2020 | December 17, 2019 | CloudFront | RTMP Support Discontinuing ([link](https://forums.aws.amazon.com/ann.jspa?annID=7356)) | |
| March 31, 2021 | March 31, 2020 | FIPS | TLS 1.2 to become the minimum for all AWS FIPS endpoints [link](https://aws.amazon.com/blogs/security/tls-1-2-to-become-the-minimum-for-all-aws-fips-endpoints/) | |
| August 1, 2021 | August 1, 2020 | Config | Indirect relationship recording removed from EC2s ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/42)) | |
