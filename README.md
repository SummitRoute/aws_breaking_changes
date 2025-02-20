# AWS breaking changes and price increases
[![feed](https://github.com/SummitRoute/aws_breaking_changes/raw/main/screenshots/feed_icon.png) Atom feed](https://github.com/SummitRoute/aws_breaking_changes/releases.atom)

This list serves to document the fairly rare changes that break applications or raise prices on AWS or where AWS has shutdown a service.

My goal is to only document issues that would break people's existing applications. So if you have a running app on AWS that makes use of some AWS API calls, what are changes AWS is making that require you to change your code, reconfigure, rebuild, or redeploy your application? Can it live forever as long as your credit card works, or is AWS potentially breaking something?

Any change has the potential to break something somewhere ([xkcd.com/1172/](https://xkcd.com/1172/)), but these seem like the more impactful changes for those that use the impacted service.  These items will stay in this list until about a month after they have gone into effect, at which point they'll be moved to the [archive](archive.md).

This list will also keep track of increases in prices.  This will not track changes in pricing models. 

| Date taking effect | Date announced | Service | Change | How to check |
| ---- | ---- |---- |---- |---- | 
| January 1, 2025 | October 29, 2024 | EC2 | EC2 G3 instance family types can no longer be started. ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/114)) | |
| March 31, 2025 | September 13, 2024 | Lex V1 | No new resources can be created in Lex V1 on March 31, 2025, and on September 15, 2025 any requests will fail. ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/107)) | |
| July 31, 2025 | July 18, 2024 | QLDB | QLDB to be deprecated on July 31, 2025. ([link](https://docs.aws.amazon.com/qldb/latest/developerguide/document-history.html)) | |
| September 17, 2025 | September 17, 2024 | DeepComposer | DeepComposer will no longer be accessible on September 17, 2025 ([link](https://aws.amazon.com/blogs/machine-learning/support-for-aws-deepcomposer-ending-soon/)) | |
| September 25, 2025 | September 24, 2024 | NICE EnginFrame | NICE EnginFrame will no longer be accessible to new users ([link](https://aws.amazon.com/jp/blogs/hpc/discontinuation-of-nice-enginframe-effective-september-25th-2025/)) | |
| October 15, 2025 | October 17, 2024 | Amazon Kinesis Data Analytics for SQL | Amazon Kinesis Data Analytics for SQL will no longer allow new applications. All data will be deleted on January 27, 2026. ([link](https://aws.amazon.com/blogs/big-data/migrate-from-amazon-kinesis-data-analytics-for-sql-to-amazon-managed-service-for-apache-flink-and-amazon-managed-service-for-apache-flink-studio/)) | |
| October 31, 2025 | February 10, 2025 | Athena | Some Athena APIs being deprecated in favor of Glue ([link](https://github.com/SummitRoute/aws_breaking_changes/issues/122#issue-2843827261)) | |
| November 13, 2025 | November 13, 2024 | MediaStore | MediaStore will no longer be accessible. ([link](https://aws.amazon.com/blogs/media/support-for-aws-elemental-mediastore-ending-soon/)) | |
| November 13, 2025 | November 12, 2024 | Elastic Transcoder | Elastic Transcoder will no longer be accessible. ([link](https://aws.amazon.com/blogs/media/support-for-amazon-elastic-transcoder-ending-soon/)) | |
| November 17, 2025 | November 12, 2024 | Application Discovery | Application Discovery Service Discovery Connector will no longer be accessible. ([link](https://aws.amazon.com/blogs/migration-and-modernization/deprecation-of-aws-application-discovery-service-discovery-connector/)) | |
| December (?), 2025 | August 29, 2024 | Deepracer | Deepracer to be open-sourced and no longer exist as a service. ([link](https://aws.amazon.com/blogs/machine-learning/celebrating-the-final-aws-deepracer-league-championship-and-road-ahead/)) | |
| February 20, 2026 | August 19, 2025 | Chime | Chime, including business calling, but not the Chime SDK, is being deprecated ([link](https://aws.amazon.com/blogs/messaging-and-targeting/update-on-support-for-amazon-chime/)) | |

## Services that are deprecated without dates for degradation:
- Cognito Sync: Documentation advises not to use it. ([link](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-sync.html)


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
* [OpenSearch Service: Supported versions of OpenSearch and Elasticsearch](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/what-is.html#choosing-version)
* [RDS Aurora Versions](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/Aurora.VersionPolicy.html)
* [RDS Db2 Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Db2.Concepts.VersionMgmt.html)
* [RDS MariaDB Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/MariaDB.Concepts.VersionMgmt.html)
* [RDS MySQL Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/MySQL.Concepts.VersionMgmt.html)
* [RDS Oracle Release Notes](https://docs.aws.amazon.com/AmazonRDS/latest/OracleReleaseNotes/Welcome.html)
* [RDS SQL Server Versions](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_SQLServer.html)
