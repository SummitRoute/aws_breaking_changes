# aws_breaking_changes
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?  

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- |
| April 1, 2020 | Unknown | CloudHSM |  Gemalto Luna 5 HSM's will be terminated ([link](https://aws.amazon.com/cloudhsm/faqs-classic/)) |  |
| April 30, 2020 | April 21, 2019 | CloudFront | API calls using code prior to 2016 will not work ([link](https://forums.aws.amazon.com/ann.jspa?annID=6754), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/cloudfront_api_version.png)) | [link](https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-api-version-check/) | 
| June 24, 2020 | July 11, 2018 | S3 | Signature must be v4 ([link](https://forums.aws.amazon.com/ann.jspa?annID=5816), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/s3_sig4.png)). Any new buckets created after June 24, 2020 will not support SigV2 signed requests, although existing buckets will continue to support SigV2 while we work with customers to move off this older request signing method. | Enable CloudTrail S3 Data Events and check `additionalEventData.SignatureVersion` ([link](https://docs.aws.amazon.com/AmazonS3/latest/dev/cloudtrail-identification-sigV2.html)) |
| September 30, 2020 | April 30, 2019 | S3 | Buckets created after September 30, 2020 must be accessed in the form \<bucketname\>.s3.amazonaws.com, not s3.amazonaws.com/\<bucketname\>/ ([link](https://aws.amazon.com/blogs/aws/amazon-s3-path-deprecation-plan-the-rest-of-the-story/)) | See link |
| December 31, 2020 | December 10, 2019 | Lambda | Python 2.7 run-time being deprecated ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/34)) | |
| December 31, 2020 | December 17, 2019 | CloudFront | RTMP Support Discontinuing ([link](https://forums.aws.amazon.com/ann.jspa?annID=7356)) | |
| March 31, 2021 | March 31, 2020 | FIPS | TLS 1.2 to become the minimum for all AWS FIPS endpoints [link](https://aws.amazon.com/blogs/security/tls-1-2-to-become-the-minimum-for-all-aws-fips-endpoints/) | |
