# Document updates {#concept_px5_4kk_xdb .concept}

This topic describes the updates to the functions, syntaxes, and permissions of MaxCompute 2.0 product documentation.

## Updates in 2019 {#section_lvf_zga_xyk .section}

|Date|Feature|Category|Description|Document|
|----|-------|--------|-----------|--------|
|2019-07-25|Spark on MaxCompute|New service|Spark on MaxCompute is introduced to Alibaba Cloud regions.|[Spark on MaxCompute overview](../../../../intl.en-US/User Guide/Spark/Spark on MaxCompute overview.md#) and [Computation pricing](../../../../intl.en-US/Pricing/Computation pricing.md#)|
|2019-04-26| -   Project lifecycle-related commands
-   IPv6 address whitelists

 |New feature|You can run commands to change the lifecycle of a project and can configure an IP address whitelist that contains IPv6 addresses.|[Project operations](../../../../intl.en-US/User Guide/Common commands/Project operations.md#)|
|2019-04-18|Script Mode SQL|New feature|The SQL engine of MaxCompute supports Script Mode SQL.|[Script Mode SQL](../../../../intl.en-US/User Guide/SQL/Script Mode SQL.md#)|
|2019-04-16|Automatic routing for tunnel endpoints|New rule|If you do not configure a tunnel endpoint, you will be routed to the tunnel endpoint that serves the network where the service endpoint is located.|[Configure endpoints](../../../../intl.en-US/Prepare/Configure endpoints.md#)|
|2019-04-15|Data outflow with data protection enabled|New method|When data protection is enabled, you can configure exception policies to allow for data outflow.|[Data protection of projects](../../../../intl.en-US/Management/Configure security features/Data protection of projects.md#)|
|2019-04-11|InstanceTunnel|New feature|You can use InstanceTunnel to call an SQL instance that starts with the `SELECT` keyword and is used for querying data.|[InstanceTunnel](../../../../intl.en-US/User Guide/Data upload and download/Tunnel SDK/InstanceTunnel.md#) and [Simple download](../../../../intl.en-US/User Guide/Data upload and download/Bulk data channel SDK example/Simple download.md#)|
|2019-03-26|UDF writable parameters for Java UDX systems|New specification|Java UDX systems are enhanced to support UDF writable parameters.|[Java UDF](../../../../intl.en-US/User Guide/SQL/UDF/Java UDF.md#)|
|2019-03-26|`INTERSECT`, `MINUS`, and `EXCEPT` statements|New specification|You can run these statements to operate data.|[UNION, INTERSECT, and EXCEPT](../../../../intl.en-US/User Guide/SQL/Select Operation/UNION, INTERSECT, and EXCEPT.md#)|
|2019-03-26|`GROUPING SETS` statement|New specification|The `GROUPING SETS` statement provides the Cube and Rollup modules. With these modules, you can aggregate and analyze data of multiple dimensions without running multiple UNION ALL clauses.|[Grouping Sets](../../../../intl.en-US/User Guide/SQL/Select Operation/Grouping Sets.md#)|
|2019-01-09|Lightning|Experience optimization|The "Lightning" section has been changed to the "Overview" section. In addition, the topic that provides pricing information has been brought offline.|[Overview](../../../../intl.en-US/User Guide/Interactive SQL (Lightning)/Overview.md#)|
|2019-01-09|Spark on MaxCompute|Experience optimization|Spark on MaxCompute is an open-source framework that functions on the service level to support data processing and analysis operations. Equipped with unified computing resources and data set permissions, Spark on MaxCompute allows you to submit and run jobs while using your preferred development methods.|[Spark on MaxCompute overview](../../../../intl.en-US/User Guide/Spark/Spark on MaxCompute overview.md#)|

## Updates in 2018 {#section_3vd_szo_mvx .section}

|Date|Feature|Category|Description|Document|
|----|-------|--------|-----------|--------|
|2018-12-20|Java UDF development through Intellij IDEA|Experience optimization|You can use Intellij IDEA to develop Java UDFs.|[Use IntelliJ IDEA to develop a Java-based UDF](../../../../intl.en-US/Best Practices/Data development/Use IntelliJ IDEA to develop a Java-based UDF.md#)|
|2018-12-17|Java UDF development through Eclipse|Experience optimization|You can use Eclipse to develop Java UDFs.|[Use Eclipse to develop a Java-based UDF](../../../../intl.en-US/Best Practices/Data development/Use Eclipse to develop a Java-based UDF.md#)|
|2018-12-04|MaxCompute for EU West 1 \(London\)|New region/zone|MaxCompute is rolled out to provision services in EU West 1 \(London\). You can purchase resources and activate projects as needed on the Alibaba Cloud console of the Intl, China, or Japan edition.|[Configure endpoints](../../../../intl.en-US/Prepare/Configure endpoints.md#)|
|2018-11-26|JSON data extraction from MongoDB to MaxCompute|Experience optimization|You can use the data synchronization feature of DataWorks to extract JSON data from MongoDB to MaxCompute.|[Migrate JSON data from MongoDB to MaxCompute](../../../../intl.en-US/Best Practices/Data migration/Migrate JSON data from MongoDB to MaxCompute.md#)|
|2018-11-15|External tables|Experience optimization|The topic that describes how to process unstructured data is replaced with the "Overview of external tables" topic.|[Overview of External tables](../../../../intl.en-US/User Guide/External table/Overview of External tables.md#)|
|2018-11-13|Migration of JSON data from OSS to MaxCompute|Experience optimization|You can use the data synchronization feature of DataWorks to migrate JSON data from OSS to MaxCompute. In addition, you can use the `GET_JSON_OBJECT` function provided by MaxCompute to extract JSON data.|[Migrate JSON data from OSS to MaxCompute](../../../../intl.en-US/Best Practices/Data migration/Migrate JSON data from OSS to MaxCompute.md#)|
|2018-11-08|MaxCompute limits|Experience optimization|The original "Reading guidance" topic is replaced with the "What you must know" topic. The new topic contains limits of MaxCompute SQL, data upload and download, MapReduce, security configuration, lighting, and PyODPS, which are not provided in the original topic.|[What you must know](../../../../intl.en-US/Product Introduction/What you must know.md#)|
|2018-11-05|`cume_dist` window function of MaxCompute SQL|New feature|You can use the `cume_dist` window function to calculate the accumulative distribution of data in a group. That is, the proportion of rows with values that are smaller than or equal to the current value in all rows in the group.|[Window functions](../../../../intl.en-US/User Guide/SQL/Builtin functions/Window functions.md#)|
|2018-11-02|Dynamic partitioning based on data migration from RDS to MaxCompute|Experience optimization|You can use the data synchronization feature of DataWorks to automatically create partitions and dynamically migrate data from RDS to MaxCompute.|[Migrate data from RDS to MaxCompute to implement dynamic partitioning](../../../../intl.en-US/Best Practices/Data migration/Migrate data from RDS to MaxCompute to implement dynamic partitioning.md#)|
|2018-09-29|User Defined Type \(UDT\)|New feature|You can reference third-party classes or objects in SQL scripts to obtain the data or call the methods of these classes or objects.|[UDT](../../../../intl.en-US/User Guide/SQL/UDT.md#)|
|2018-09-29|User Defined Join \(UDJ\)|New feature|UDJ is an extension to the UDF framework of MaxCompute. With UDJ, you can define join operations and perform these join operations across tables flexibly. In addition, UDJ reduces the need for performing operations at the bottom layer of the distributed system, making the system run faster.|[UDJ](../../../../intl.en-US/User Guide/SQL/UDJ.md#)|
|2018-07-30|Solutions to long-tail traffic|Experience optimization|The documentation is updated to describe typical long-tail traffic issues and the corresponding solutions.|[Optimize long tail computing](../../../../intl.en-US/Best Practices/Compute optimization/Optimize long tail computing.md#)|
|2018-05-25|GZIP compression|New feature|MaxCompute can use its built-in extractor to read CSV or TSV data that is compressed by using GZIP from OSS. An uncompressed file differs from a compressed file in their SERDEPROPERTIES attributes.|[Access OSS unstructured data](../../../../intl.en-US/User Guide/External table/Access OSS unstructured data.md#)|
|2018-05-25|Hive|New specification|With Hive, you can use the unstructured data framework of MaxCompute to process the data that is stored on OSS in a variety of open-source formats such as ORC, PARQUET, SEQUENCEFILE, RCFILE, AVRO, and TEXTFILE.|[Processing open source format data for OSS](../../../../intl.en-US/User Guide/External table/Processing open source format data for OSS.md#)|
|2018-05-25|`SELECT TRANSFORM` statement|New feature|The `SELECT TRANSFORM` statement simplifies code reference and script compilation. It supports a wide range of programming languages such as Java, Python, Shell, and Perl, helping you to develop ad hoc functions.|[SELECT TRANSFORM](../../../../intl.en-US/User Guide/SQL/Select Operation/SELECT TRANSFORM.md#)|
|2018-05-25|`SEMI JOIN` statement|New feature|In a `SEMI JOIN` statement, the right-side table is used only to filter the data from the left-side table and will not be presented in the result set. This statement supports two clauses: `LEFT SEMI JOIN` and `LEFT ANTI JOIN`.|[SEMI JOIN](../../../../intl.en-US/User Guide/SQL/Select Operation/SEMI JOIN.md#)|
|2018-05-25|Implicit type conversion in `CASE WHEN` expressions|New specification|MaxCompute SQL allows for implicit type conversion in `CASE WHEN` expressions.|[Type conversions](../../../../intl.en-US/User Guide/SQL/Type conversions.md#)|
|2018-05-16|Full table scan|New feature|You can enable and set the full table scan function.|[Other operations](../../../../intl.en-US/User Guide/Common commands/Other operations.md#)|
|2018-04-14|Renewal of expired instances through Auto-Renew|New specification|When your **Subscription** instance expires, you can renew it through the **Auto-Renew** option on the MaxCompute console.|None|
|2018-04-10|MaxCompute for US East 1 \(Virginia\)|New region/zone|MaxCompute is rolled out to provision services in US East 1 \(Virginia\). You can purchase resources and activate projects as needed on the Alibaba Cloud console of the Intl, China, or Japan edition.|[Configure endpoints](../../../../intl.en-US/Prepare/Configure endpoints.md#)|
|2018-04-02|MaxCompute Studio 2.9.0|New feature|MaxCompute Studio 2.9.0 enables you to check and rectify code, develop and debug graphs, and fix errors. For more information, see [MaxCompute Studio 2.9.0](https://plugins.jetbrains.com/plugin/9193-maxcompute-studio/update/44687).|[What is Studio](../../../../intl.en-US/Tools and Downloads/MaxCompute Studio/What is Studio.md#)|
|2018-03-28|MaxCompute Manager for China East 1 \(Hangzhou\)|New specification|Enterprise customers who use the Subscription billing method in China East 1 \(Hangzhou\) can get their computing resource usage and task queuing information. In addition, MaxCompute Manager can manage computing tasks by group based on task priorities.|[MaxCompute Manager](../../../../intl.en-US/Workbench/MaxCompute Manager.md#)|
|2018-03-23|Tunnel endpoint customization in MaxCompute Studio|Defect rectification|When you use Instance Tunnel to download SQL query results, you can specify a tunnel endpoint.|[Configure endpoints](../../../../intl.en-US/Prepare/Configure endpoints.md#)|
|2018-03-22|MaxCompute for China East 1 \(Hangzhou\)|New region/zone|MaxCompute is rolled out in China East 1 \(Hangzhou\) to provision services. You can purchase resources and activate projects as needed on the Alibaba Cloud console of the Intl, China, or Japan edition.|[Configure endpoints](../../../../intl.en-US/Prepare/Configure endpoints.md#)|
|2018-02-09|PyODPS 0.7.15|New version/New specification|The relevant features in PyODPS 0.7.15 are optimized or rectified and new features are introduced to enhance development experience and efficiency: -   You can use DataFrame to define functions based on Python 3.6.
-   The defect due to which the functions that you define through DataFrame in Python 3.5 incur errors is fixed.
-   You can set the parameters that determine the running of XFlow when XFlow is operating.
-   When you create a PyODPS DataFrame from a Pandas DataFrame, you can use the as\_type parameter to specify the combination type, for example, LIST or DICT.

 |[Python SDK](../../../../intl.en-US/SDK Reference /Python SDK.md#)|
|2018-02-09|MaxCompute for Asia Pacific SE 5 \(Jakarta\)|New region/zone|MaxCompute is rolled out to provision services in Asia Pacific SE 5 \(Jakarta\). You can purchase resources and activate projects as needed on the Alibaba Cloud console of the Intl, China, or Japan edition.|[Configure endpoints](../../../../intl.en-US/Prepare/Configure endpoints.md#)|
|2018-02-03|MaxCompute Studio 2.8.2.3|Experience optimization| -   In the left-side pane of the MaxCompute Studio Editor, you can directly run an SQL statement without clicking any button in the toolbar.
-   In the MaxCompute Studio Project Explorer, built-in functions are classified by type to help you easily find a specific function.

 |None|
|2018-02-03|top instance command|New feature|The documentation is updated to describe the top instance command.|[Instances operations](../../../../intl.en-US/User Guide/Common commands/Instances operations.md#)|
|2018-02-03|external info query|New feature|The documentation is updated to describe the external info element, including LOCATION and StorageHandler, of external tables.|[Table operations](../../../../intl.en-US/User Guide/Common commands/Table operations.md#) and [Access OSS unstructured data](../../../../intl.en-US/User Guide/External table/Access OSS unstructured data.md#)|
|2018-02-01|top instance command|New specification|In MaxCompute Console 0.29.0, you can run the top instance command to obtain information about the jobs that running or waiting in the queue.|[Instances operations](../../../../intl.en-US/User Guide/Common commands/Instances operations.md#)|
|2018-01-31|MaxCompute Manager|New feature|Enterprise customers who use the Subscription billing method can get their computing resource usage and task queuing information. In addition, MaxCompute Manager can manage computing tasks by group based on task priorities.|[MaxCompute Manager](../../../../intl.en-US/Workbench/MaxCompute Manager.md#)|
|2018-01-22|DataHub for four regions|New region/zone|DataHub is introduced to four regions: China East 2 \(Shanghai\), China North 2 \(Beijing\), China South 1 \(Shenzhen\), and Asia Pacific SE 1 \(Singapore\).|None|
|2018-01-18|MaxCompute Studio 2.8.2.2|New version/New specification|MaxCompute Studio 2.8.2.2 provides the following functions: -   Develop Python UDFs.
-   Compile unstructured unit tests.
-   Operate complex data types while running UDFs on your computer.
-   Define SQL statement format rules.

 |[What is Studio](../../../../intl.en-US/Tools and Downloads/MaxCompute Studio/What is Studio.md#)|
|2018-01-18|MaxCompute for Asia Pacific SOU 1 \(Mumbai\)|New region/zone|MaxCompute is rolled out in Asia Pacific SOU 1 \(Mumbai\) to provision services. You can purchase resources and activate projects as needed on the Alibaba Cloud console of the Intl, China, or Japan edition.|[Configure endpoints](../../../../intl.en-US/Prepare/Configure endpoints.md#)|
|2018-01-10|Full table scan|New feature|The full table scan function is forbidden by MaxCompute so as to avoid resource waste and reduce costs.|[Project operations](../../../../intl.en-US/User Guide/Common commands/Project operations.md#)|
|2018-01|Project data protection|Experience optimization|The documentation is updated to describe the background information and mechanism of data protection as well as how to allow for data outflow when the data protection mechanism is enabled.|[Data protection of projects](../../../../intl.en-US/Management/Configure security features/Data protection of projects.md#)|
|2018-01|Hive UDF|Experience optimization|An example is added to describe how to use Hive UDFs in MaxCompute.|[Java UDF](../../../../intl.en-US/User Guide/SQL/UDF/Java UDF.md#)|
|2018-01|TableTunnel|Experience optimization|The documentation is updated to describe TableTunnel, its limits, and how it works at the bottom layer.|[TableTunnel](../../../../intl.en-US/User Guide/Data upload and download/Tunnel SDK/TableTunnel.md#)|
|2018-01|Full table scan|New feature|The documentation is updated to describe the full table scan function.|[Announcements](intl.en-US/Release Note/Announcements.md#), [Other operations](../../../../intl.en-US/User Guide/Common commands/Other operations.md#), and [SQL Common Errors](https://www.alibabacloud.com/help/doc-detail/64654.htm?spm=a2c63.p38356.b99.300.1d917e25MeqtWV)|
