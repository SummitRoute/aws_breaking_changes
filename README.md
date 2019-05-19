# aws_breaking_changes
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?  

Any change has the potential to break something somewhere, but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be removed.

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- |
| May 30, 2019 | Unknown | Lambda | Support ends for runtimes Node.js 6.10 and .NET Core 2.0; no longer able to update ([link](https://docs.aws.amazon.com/lambda/latest/dg/runtime-support-policy.html)) | `aws lambda list-functions --query 'Functions[?Runtime == `nodejs6.10`]'.FunctionName` |
| June 1, 2019 | March 25, 2019 | Mechanical Turk | Older versions of the MTurk Requester API (2014-08-15) will stop working ([link](https://forums.aws.amazon.com/ann.jspa?annID=6686)) | TODO | 
| June 11, 2019 | May 14, 2019 | Lambda | Execution environment update to Amazon Linux 2018.03 ([link](https://aws.amazon.com/blogs/compute/upcoming-updates-to-the-aws-lambda-execution-environment/)) | See link |
| June 24, 2019 | July 11, 2018 | S3 | Signature must be v4 ([link](https://forums.aws.amazon.com/ann.jspa?annID=5816), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/s3_sig4.png)) | Enable CloudTrail S3 Data Events and check `additionalEventData.SignatureVersion` ([link](https://docs.aws.amazon.com/AmazonS3/latest/dev/cloudtrail-identification-sigV2.html)) |
| October 16, 2019 | Unknown | Elastic Beanstalk | Windows Server 2008 R2 retired ([link](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/platforms-support-policy.html)) | TODO |
| March 1, 2020 | Unknown | Elastic Beanstalk | Apache HTTP Server 2.2, Nginx 1.12.2, GlassFish 4.x, Go 1.3–1.10, Java 6, Node.js 4.x–8.x, PHP 5.4–5.6, PHP 7.0–7.1, Python 2.6, 2.7, 3.4, Ruby 1.9.3, Ruby 2.0–2.3, Tomcat 6, Tomcat 8 ([link](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/platforms-support-policy.html)) | TODO |
| April 1, 2020 | Unknown | CloudHSM |  Gemalto Luna 5 HSM's will be terminated ([link](https://aws.amazon.com/cloudhsm/faqs-classic/)) | TODO |
| April 30, 2020 | April 21, 2019 | CloudFront | API calls using code prior to 2016 will not work ([link](https://forums.aws.amazon.com/ann.jspa?annID=6754), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/cloudfront_api_version.png)) | [link](https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-api-version-check/) | 
| September 30, 2020 | April 30, 2019 | S3 | Buckets created after September 30, 2020 must be accessed in the form \<bucketname\>.s3.amazonaws.com, not s3.amazonaws.com/\<bucketname\>/ ([link](https://aws.amazon.com/blogs/aws/amazon-s3-path-deprecation-plan-the-rest-of-the-story/)) | See link |
