# Amazon Kinesis Data Streams Developer Guide

-----
*****Copyright &copy; 2019 Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What Is Amazon Kinesis Data Streams?](introduction.md)
   + [Kinesis Data Streams Key Concepts](key-concepts.md)
   + [Creating and Updating Data Streams](amazon-kinesis-streams.md)
   + [Kinesis Data Streams Producers](amazon-kinesis-producers.md)
   + [Kinesis Data Streams Consumers](amazon-kinesis-consumers.md)
   + [Kinesis Data Streams Limits](service-sizes-and-limits.md)
+ [Getting Started Using Amazon Kinesis Data Streams](getting-started.md)
   + [Setting Up for Amazon Kinesis Data Streams](before-you-begin.md)
   + [Tutorial: Visualizing Web Traffic Using Amazon Kinesis Data Streams](kinesis-sample-application.md)
   + [Tutorial: Getting Started With Amazon Kinesis Data Streams Using AWS CLI](kinesis-tutorial-cli.md)
      + [Install and Configure the AWS CLI](kinesis-tutorial-cli-installation.md)
      + [Perform Basic Stream Operations](fundamental-stream.md)
   + [Tutorial: Analyzing Real-Time Stock Data Using Kinesis Data Streams](learning-kinesis-module-one.md)
      + [Prerequisites](learning-kinesis-module-one-begin.md)
      + [Step 1: Create a Data Stream](learning-kinesis-module-one-create-stream.md)
      + [Step 2: Create an IAM Policy and User](learning-kinesis-module-one-iam.md)
      + [Step 3: Download and Build the Implementation Code](learning-kinesis-module-one-download.md)
      + [Step 4: Implement the Producer](learning-kinesis-module-one-producer.md)
      + [Step 5: Implement the Consumer](learning-kinesis-module-one-consumer.md)
      + [Step 6: (Optional) Extending the Consumer](learning-kinesis-module-one-consumer-extension.md)
      + [Step 7: Finishing Up](learning-kinesis-module-one-finish.md)
+ [Creating and Managing Streams](working-with-streams.md)
   + [Creating a Stream](kinesis-using-sdk-java-create-stream.md)
   + [Listing Streams](kinesis-using-sdk-java-list-streams.md)
   + [Listing Shards](kinesis-using-sdk-java-list-shards.md)
   + [Retrieving Shards from a Stream](kinesis-using-sdk-java-retrieve-shards.md)
   + [Deleting a Stream](kinesis-using-sdk-java-delete-stream.md)
   + [Resharding a Stream](kinesis-using-sdk-java-resharding.md)
      + [Strategies for Resharding](kinesis-using-sdk-java-resharding-strategies.md)
      + [Splitting a Shard](kinesis-using-sdk-java-resharding-split.md)
      + [Merging Two Shards](kinesis-using-sdk-java-resharding-merge.md)
      + [After Resharding](kinesis-using-sdk-java-after-resharding.md)
   + [Changing the Data Retention Period](kinesis-extended-retention.md)
   + [Tagging Your Streams in Amazon Kinesis Data Streams](tagging.md)
   + [Monitoring Streams in Amazon Kinesis Data Streams](monitoring.md)
      + [Monitoring the Amazon Kinesis Data Streams Service with Amazon CloudWatch](monitoring-with-cloudwatch.md)
      + [Monitoring Kinesis Data Streams Agent Health with Amazon CloudWatch](agent-health.md)
      + [Logging Amazon Kinesis Data Streams API Calls with AWS CloudTrail](logging-using-cloudtrail.md)
      + [Monitoring the Kinesis Client Library with Amazon CloudWatch](monitoring-with-kcl.md)
      + [Monitoring the Kinesis Producer Library with Amazon CloudWatch](monitoring-with-kpl.md)
   + [Controlling Access to Amazon Kinesis Data Streams Resources Using IAM](controlling-access.md)
   + [Using Server-Side Encryption](server-side-encryption.md)
      + [What Is Server-Side Encryption for Kinesis Data Streams?](what-is-sse.md)
      + [Costs, Regions, and Performance Considerations](costs-performance.md)
      + [How Do I Get Started with Server-Side Encryption?](getting-started-with-sse.md)
      + [Creating and Using User-Generated KMS Master Keys](creating-using-sse-master-keys.md)
      + [Permissions to Use User-Generated KMS Master Keys](permissions-user-key-KMS.md)
      + [Verifying and Troubleshooting KMS Key Permissions](sse-troubleshooting.md)
   + [Using Amazon Kinesis Data Streams with Interface VPC Endpoints](vpc.md)
   + [Managing Kinesis Data Streams Using the Console](managing-streams-console.md)
+ [Writing Data to Amazon Kinesis Data Streams](building-producers.md)
   + [Developing Producers Using the Amazon Kinesis Producer Library](developing-producers-with-kpl.md)
      + [Installing the KPL](kinesis-kpl-dl-install.md)
      + [Transitioning to Amazon Trust Services (ATS) Certificates for the Kinesis Producer Library](kinesis-kpl-upgrades.md)
      + [KPL Supported Platforms](kinesis-kpl-supported-plats.md)
      + [KPL Key Concepts](kinesis-kpl-concepts.md)
      + [Integrating the KPL with Producer Code](kinesis-kpl-integration.md)
      + [Writing to your Kinesis Data Stream Using the KPL](kinesis-kpl-writing.md)
      + [Configuring the Kinesis Producer Library](kinesis-kpl-config.md)
      + [Consumer De-aggregation](kinesis-kpl-consumer-deaggregation.md)
      + [Using the KPL with Kinesis Data Firehose](kpl-with-firehose.md)
   + [Developing Producers Using the Amazon Kinesis Data Streams API with the AWS SDK for Java](developing-producers-with-sdk.md)
   + [Writing to Amazon Kinesis Data Streams Using Kinesis Agent](writing-with-agents.md)
   + [Troubleshooting Amazon Kinesis Data Streams Producers](troubleshooting-producers.md)
   + [Advanced Topics for Kinesis Data Streams Producers](advanced-producers.md)
      + [KPL Retries and Rate Limiting](kinesis-producer-adv-retries-rate-limiting.md)
      + [Considerations When Using KPL Aggregation](kinesis-producer-adv-aggregation.md)
+ [Reading Data from Amazon Kinesis Data Streams](building-consumers.md)
   + [Developing Amazon Kinesis Data Streams Consumers](shared-fan-out-consumers.md)
      + [Developing Consumers Using the Kinesis Client Library 1.x](developing-consumers-with-kcl.md)
         + [Developing a Kinesis Client Library Consumer in Java](kinesis-record-processor-implementation-app-java.md)
         + [Developing a Kinesis Client Library Consumer in Node.js](kinesis-record-processor-implementation-app-nodejs.md)
         + [Developing a Kinesis Client Library Consumer in .NET](kinesis-record-processor-implementation-app-dotnet.md)
         + [Developing a Kinesis Client Library Consumer in Python](kinesis-record-processor-implementation-app-py.md)
         + [Developing a Kinesis Client Library Consumer in Ruby](kinesis-record-processor-implementation-app-ruby.md)
      + [Developing Consumers Using the Kinesis Client Library 2.0](developing-consumers-with-kcl-v2.md)
         + [Developing a Kinesis Client Library Consumer in Java](kcl2-standard-consumer-java-example.md)
         + [Developing a Kinesis Client Library Consumer in Python](kcl2-standard-consumer-python-example.md)
      + [Developing Consumers Using the Kinesis Data Streams API with the AWS SDK for Java](developing-consumers-with-sdk.md)
   + [Using Consumers with Enhanced Fan-Out](introduction-to-enhanced-consumers.md)
      + [Developing Consumers with Enhanced Fan-Out Using the Kinesis Client Library 2.0](building-enhanced-consumers-kcl.md)
         + [Developing a Consumer Using the Kinesis Client Library 2.x in Java](building-enhanced-consumers-kcl-java.md)
      + [Developing Consumers with Enhanced Fan-Out Using the Kinesis Data Streams API](building-enhanced-consumers-api.md)
      + [Managing Consumers with Enhanced Fan-Out Using the AWS Management Console](building-enhanced-consumers-console.md)
   + [Migrating from Kinesis Client Library 1.x to 2.x](kcl-migration.md)
   + [Developing Consumers Using Amazon Kinesis Data Analytics](kda-consumer.md)
   + [Developing Consumers Using Amazon Kinesis Data Firehose](kdf-consumer.md)
   + [Developing Consumers Using AWS Lambda](lambda-consumer.md)
   + [Troubleshooting Amazon Kinesis Data Streams Consumers](troubleshooting-consumers.md)
   + [Advanced Topics for Amazon Kinesis Data Streams Consumers](advanced-consumers.md)
      + [Tracking Amazon Kinesis Data Streams Application State](kinesis-record-processor-ddb.md)
      + [Low-Latency Processing](kinesis-low-latency.md)
      + [Using AWS Lambda with the Kinesis Producer Library](kinesis-record-deaggregation.md)
      + [Resharding, Scaling, and Parallel Processing](kinesis-record-processor-scaling.md)
      + [Handling Duplicate Records](kinesis-record-processor-duplicates.md)
      + [Recovering from Failures in Amazon Kinesis Data Streams](kinesis-record-processor-failover-recovery.md)
      + [Handling Startup, Shutdown, and Throttling](kinesis-record-processor-additional-considerations.md)
+ [Document History](history.md)
+ [AWS Glossary](glossary.md)