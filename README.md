# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices on AWS or where AWS has shutdown a service.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere ([xkcd.com/1172/](https://xkcd.com/1172/)), but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| April 6(?), 2024 | Unknown | Snowmobile |  All references to the AWS Snowmobile service have been scrubbed from the docs. This has occured at some point between Feb 27, 2024 and April 6, 2024. This service appears to have been silently deprecated. | |
| April 24(?), 2024 | Unknown | Workdocs | The documentation now states new users cannot sign up, and emails were sent to customers informing them that their data will be deleted on April 26, 2025 ([link](https://twitter.com/iann0036/status/1783618453343219994))| |
| May 5, 2024 | May 10, 2023 | OpsWorks |  OpsWorks for Chef Automate will no longer be able to be used ([link](https://docs.aws.amazon.com/opsworks/latest/userguide/welcome_classic.html)) | |
| May 26, 2024 | May 25, 2023 | OpsWorks |  OpsWorks Stacks will no longer be able to be used ([link](https://docs.aws.amazon.com/opsworks/latest/userguide/welcome_classic.html)) | |
| June 6, 2024 | July 30, 2024 | CodeCommit | CodeCommit stopped being available to new accounts without announcement, but still works for existing customers.  ([link](https://repost.aws/questions/QUshILm0xbTjWJZSD8afYVgA/codecommit-cannot-create-a-repository)) Later announced as discontinued for new customers. ([link](https://x.com/jeffbarr/status/1818488419347317217)) | |
| July 22, 2024 | N/A | Mobile Hub | Mobile Hub removed from the SDK. ([link](https://github.com/aws/aws-sdk-go/commit/e8ff775f9a1995a3e9654b6631d745e94fd32742) | |
| July 29(?), 2024 | July 30, 2024 | CloudSearch | Access discontinued for new customers ([link](https://dev.classmethod.jp/articles/aws-start-to-restrict-codecommit-and-cloudsearch/)) | |
| July 29(?), 2024 | July 30, 2024 | Cloud9 |Access discontinued for new customers ([link](https://dev.classmethod.jp/articles/aws-start-to-restrict-codecommit-and-cloudsearch/)) | |
| July 30(?), 2024 | July 30, 2024 | SimpleDB | Access discontinued for new customers ([link](https://x.com/jeffbarr/status/1818488419347317217)) | |
| July 30(?), 2024 | July 30, 2024 | S3 Select | Access discontinued for new customers ([link](https://x.com/jeffbarr/status/1818488419347317217)) | |
| July 30(?), 2024 | July 30, 2024 | Forecast | Access discontinued for new customers ([link](https://x.com/jeffbarr/status/1818488419347317217)) | |
| July 30(?), 2024 | July 30, 2024 | Data Pipeline | Access discontinued for new customers ([link](https://x.com/jeffbarr/status/1818488419347317217)) | |
| July 31, 2024 | July 31, 2023 | CodeStar | AWS CodeStar is being deprecated. Existing resources will be unaffected, but you will not be able to create new resources with it. ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/84#issue-1830512424)) | |
| September 30, 2024 | November 22, 2023 | Application Cost Profiler (ACP) | AWS Application Cost Profiler (ACP) will be discontinued ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/87)) | |
| October 1, 2024 | October 20, 2021 | EC2 Auto Scaling Launch Configurations | Through a series of deprecations spanning multiple years, AWS is slowly killing off EC2 Auto Scaling Launch Configurations in favor of EC2 Launch Templates.  On October 1, 2024, only those accounts that have previously used Launch Configurations can continue to do so.  A final deprecation has not yet been announced.   ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/95)) ([Original soft deprecation](https://aws.amazon.com/blogs/compute/amazon-ec2-auto-scaling-will-no-longer-add-support-for-new-ec2-features-to-launch-configurations/)) | |
| November 29, 2024 | Unknown | Finspace | FinSpace Dataset Browser will be discontinued ([link](https://docs.aws.amazon.com/finspace/latest/management-api/API_UpdateEnvironment.html)) | |
| December 16, 2024 | Unknown | IoT 1-Click | AWS IoT 1-Click service will be discontinued ([link](https://docs.aws.amazon.com/iot-1-click/latest/developerguide/1click-end-of-life.html)) | |
| December 31, 2024 | December 28, 2023 | Aurora Serverless v1 | Aurora Serverless will be automatically upgraded to v2, which has some significant differences, such as not scaling down to zero. ([link](https://twitter.com/jeremy_daly/status/1740475761113604451)) | |
| July 31, 2025 | July 18, 2024 | QLDB | QLDB to be deprecated on July 31, 2025. ([link](https://docs.aws.amazon.com/qldb/latest/developerguide/document-history.html)) | |

## AWS support calendars for third-party products

Services such as Lambda and RDS provide managed hosting for third-party products that have their own lifecycle.

AWS already publishes the support calendar for those products.

If you use one of these services and need to know when AWS will stop supporting your current version you can consult its calendar directly.

* [Amazon Linux Release Cadence](https://docs.aws.amazon.com/linux/al2023/ug/release-cadence.html)
* [Elasticache Redis supported versions](https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/supported-engine-versions.html)
* [Elasticache Memcached suppported versions](https://docs.aws.amazon.com/AmazonElastiCache/latest/mem-ug/supported-engine-versions-mc.html)
* [EKS Kubernetes release calendar](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html)
* [Lambda supported runtimes](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html) (major versions for all languages)
* [Lambda runtime updates](https://docs.aws.amazon.com/lambda/latest/dg/runtimes-update.html) (info to control patch versions)
* [RDS Aurora Versions](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/Aurora.VersionPolicy.html)
* [RDS Db2 Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Db2.Concepts.VersionMgmt.html)
* [RDS MariaDB Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/MariaDB.Concepts.VersionMgmt.html)
* [RDS MySQL Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/MySQL.Concepts.VersionMgmt.html)
* [RDS Oracle Release Notes](https://docs.aws.amazon.com/AmazonRDS/latest/OracleReleaseNotes/Welcome.html)
* [RDS SQL Server Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_SQLServer.html)
