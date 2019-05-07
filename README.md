# aws_breaking_changes

[![feed](https://aleen42.github.io/badges/src/rss.svg)](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

List of changes announced for AWS that may break existing code due to deprecations or otherwise.

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- |
| May 30, 2019 | Unknown | Lambda | Support ends for runtimes Node.js 6.10 and .NET Core 2.0; no longer able to update ([link](https://docs.aws.amazon.com/lambda/latest/dg/runtime-support-policy.html)) | `aws lambda list-functions --query 'Functions[?Runtime == `nodejs6.10`]'.FunctionName` |
| June 1, 2019 | March 25, 2019 | Mechanical Turk | Older versions of the MTurk Requester API (2014-08-15) will stop working ([link](https://forums.aws.amazon.com/ann.jspa?annID=6686)) | TODO | 
| June 24, 2019      | July 11, 2018  | S3 | Signature must be v4 ([link](https://forums.aws.amazon.com/ann.jspa?annID=5816), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/s3_sig4.png)) | Enable CloudTrail S3 Data Events and check `additionalEventData.SignatureVersion` ([link](https://docs.aws.amazon.com/AmazonS3/latest/dev/cloudtrail-identification-sigV2.html)) |
| April 30, 2020 | April 21, 2019 | CloudFront | API calls using code prior to 2016 will not work ([link](https://forums.aws.amazon.com/ann.jspa?annID=6754), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/cloudfront_api_version.png)) | [link](https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-api-version-check/) | 
| September 30, 2020 | April 30, 2019 | S3 | Paths must be accessed in the form \<bucketname\>.s3.amazonaws.com, not s3.amazonaws.com/\<bucketname\>/ ([link](https://forums.aws.amazon.com/ann.jspa?annID=6776), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/s3_path_format.png)). | TODO |
