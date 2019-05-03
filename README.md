# aws_breaking_changes
List of changes announced for AWS that may break existing code due to deprecations or otherwise.

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- |
| May 30, 2019 | Unknown | Lambda | Support ends for runtimes Node.js 6.10 .NET Core 2.0, no longer able to update ([link](https://docs.aws.amazon.com/lambda/latest/dg/runtime-support-policy.html)) | TODO |
| June 24, 2019      | July 11, 2018  | S3 | Signature must be v4 ([link](https://forums.aws.amazon.com/ann.jspa?annID=5816), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/s3_sig4.png)) | TODO |
| April 30, 2020 | April 21, 2019 | CloudFront | API calls using code prior to 2016 will not work ([link](https://forums.aws.amazon.com/ann.jspa?annID=6754), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/cloudfront_api_version.png)) | [link](https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-api-version-check/) | 
| September 30, 2020 | April 30, 2019 | S3 | Paths must be in the form \<bucketname\>.s3.amazonaws.com, not s3.amazonaws.com/\<bucketname\>/ ([link](https://forums.aws.amazon.com/ann.jspa?annID=6776), [screenshot](https://github.com/SummitRoute/aws_breaking_changes/raw/master/screenshots/s3_path_format.png)). This will break buckets with periods in them. | TODO |
