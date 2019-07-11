After items are a month old, they'll be moved to this page, to archive them.

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- |
| May 30, 2019 | Unknown | Lambda | Support ends for runtime .NET Core 2.0; no longer able to update ([link](https://docs.aws.amazon.com/lambda/latest/dg/runtime-support-policy.html)) | ``aws lambda list-functions --query 'Functions[?Runtime == `dotnetcore2.0`]'.FunctionName`` |
| June 1, 2019 | March 25, 2019 | Mechanical Turk | Older versions of the MTurk Requester API (2014-08-15) will stop working ([link](https://forums.aws.amazon.com/ann.jspa?annID=6686)) |  | 
| June 11, 2019 | May 14, 2019 | Lambda | Execution environment update to Amazon Linux 2018.03 ([link](https://aws.amazon.com/blogs/compute/upcoming-updates-to-the-aws-lambda-execution-environment/)) | See link |