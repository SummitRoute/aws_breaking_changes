# aws_breaking_changes
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?  

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- |
| January 6, 2020 | October 18, 2019 | Lambda | Support ends for Node.js 8.10, no longer able to create functions. Feb 3, no longer able to create. ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/27)) |  |
| March 1, 2020 | Unknown | Elastic Beanstalk | Apache HTTP Server 2.2, Nginx 1.12.2, GlassFish 4.x, Go 1.3–1.10, Java 6, Node.js 4.x–8.x, PHP 5.4–5.6, PHP 7.0–7.1, Python 2.6, 2.7, 3.4, Ruby 1.9.3, Ruby 2.0–2.3, Tomcat 6, Tomcat 8 ([link](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/platforms-support-policy.html)) |  |
| April 1, 2020 | Unknown | CloudHSM |  Gemalto Luna 5 HSM's will be terminated ([link](https://aws.amazon.com/cloudhsm/faqs-classic/)) |  |
| April 30, 2020 | April 21, 2019 | CloudFront | API calls using code prior to 2016 will not work ([link](https://forums.aws.amazon.com/ann.jspa?annID=6754), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/cloudfront_api_version.png)) | [link](https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-api-version-check/) | 
| June 24, 2020 | July 11, 2018 | S3 | Signature must be v4 ([link](https://forums.aws.amazon.com/ann.jspa?annID=5816), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/s3_sig4.png)). Any new buckets created after June 24, 2020 will not support SigV2 signed requests, although existing buckets will continue to support SigV2 while we work with customers to move off this older request signing method. | Enable CloudTrail S3 Data Events and check `additionalEventData.SignatureVersion` ([link](https://docs.aws.amazon.com/AmazonS3/latest/dev/cloudtrail-identification-sigV2.html)) |
| September 30, 2020 | April 30, 2019 | S3 | Buckets created after September 30, 2020 must be accessed in the form \<bucketname\>.s3.amazonaws.com, not s3.amazonaws.com/\<bucketname\>/ ([link](https://aws.amazon.com/blogs/aws/amazon-s3-path-deprecation-plan-the-rest-of-the-story/)) | See link |
