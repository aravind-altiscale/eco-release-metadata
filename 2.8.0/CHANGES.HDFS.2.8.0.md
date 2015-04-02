# Hadoop Changelog

## Release 2.8.0 - Unreleased

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HDFS-8009](https://issues.apache.org/jira/browse/HDFS-8009) | Signal congestion on the DataNode |  Major | datanode | Haohui Mai | Haohui Mai |
| [HDFS-8008](https://issues.apache.org/jira/browse/HDFS-8008) | Support client-side back off when the datanodes are congested |  Major | hdfs-client | Haohui Mai | Haohui Mai |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HDFS-8004](https://issues.apache.org/jira/browse/HDFS-8004) | Use KeyProviderCryptoExtension#warmUpEncryptedKeys when creating an encryption zone |  Trivial | encryption | Andrew Wang | Andrew Wang |
| [HDFS-7978](https://issues.apache.org/jira/browse/HDFS-7978) | Add LOG.isDebugEnabled() guard for some LOG.debug(..) |  Major | . | Walter Su | Walter Su |
| [HDFS-7944](https://issues.apache.org/jira/browse/HDFS-7944) | Minor cleanup of BlockPoolManager#getAllNamenodeThreads |  Minor | . | Arpit Agarwal | Arpit Agarwal |
| [HDFS-7928](https://issues.apache.org/jira/browse/HDFS-7928) | Scanning blocks from disk during rolling upgrade startup takes a lot of time if disks are busy |  Major | datanode | Rushabh S Shah | Rushabh S Shah |
| [HDFS-7890](https://issues.apache.org/jira/browse/HDFS-7890) | Improve information on Top users for metrics in RollingWindowsManager and lower log level |  Major | . | J.Andreina | J.Andreina |
| [HDFS-7875](https://issues.apache.org/jira/browse/HDFS-7875) | Improve log message when wrong value configured for dfs.datanode.failed.volumes.tolerated |  Trivial | datanode | nijel | nijel |
| [HDFS-7835](https://issues.apache.org/jira/browse/HDFS-7835) | make initial sleeptime in locateFollowingBlock configurable for DFSClient. |  Major | hdfs-client | zhihai xu | zhihai xu |
| [HDFS-7829](https://issues.apache.org/jira/browse/HDFS-7829) | Code clean up for LocatedBlock |  Minor | . | Jing Zhao | Takanobu Asanuma |
| [HDFS-7793](https://issues.apache.org/jira/browse/HDFS-7793) | Refactor DFSOutputStream separating DataStreamer out |  Major | hdfs-client | Kai Zheng | Li Bo |
| [HDFS-7671](https://issues.apache.org/jira/browse/HDFS-7671) | hdfs user guide should point to the common rack awareness doc |  Major | documentation | Allen Wittenauer | Kai Sasaki |
| [HDFS-7645](https://issues.apache.org/jira/browse/HDFS-7645) | Rolling upgrade is restoring blocks from trash multiple times |  Major | datanode | Nathan Roberts | Keisuke Ogiwara |
| [HDFS-4396](https://issues.apache.org/jira/browse/HDFS-4396) | Add START\_MSG/SHUTDOWN\_MSG for ZKFC |  Major | auto-failover, ha, tools | Liang Xie | Liang Xie |
| [HDFS-3918](https://issues.apache.org/jira/browse/HDFS-3918) | EditLogTailer shouldn't log WARN when other node is in standby mode |  Major | ha | Todd Lipcon | Todd Lipcon |
| [HDFS-2360](https://issues.apache.org/jira/browse/HDFS-2360) | Ugly stacktrace when quota exceeds |  Minor | hdfs-client | Rajit Saha | Harsh J |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HDFS-8026](https://issues.apache.org/jira/browse/HDFS-8026) | Trace FSOutputSummer#writeChecksumChunks rather than DFSOutputStream#writeChunk |  Minor | . | Colin Patrick McCabe | Colin Patrick McCabe |
| [HDFS-8002](https://issues.apache.org/jira/browse/HDFS-8002) | Website refers to /trash directory |  Major | documentation | Mike Drob | Brahma Reddy Battula |
| [HDFS-7997](https://issues.apache.org/jira/browse/HDFS-7997) | The first non-existing xattr should also throw IOException |  Minor | . | zhouyingchao | zhouyingchao |
| [HDFS-7990](https://issues.apache.org/jira/browse/HDFS-7990) | IBR delete ack should not be delayed |  Major | namenode | Daryn Sharp | Daryn Sharp |
| [HDFS-7922](https://issues.apache.org/jira/browse/HDFS-7922) | ShortCircuitCache#close is not releasing ScheduledThreadPoolExecutors |  Major | . | Rakesh R | Rakesh R |
| [HDFS-7916](https://issues.apache.org/jira/browse/HDFS-7916) | 'reportBadBlocks' from datanodes to standby Node BPServiceActor goes for infinite loop |  Critical | datanode | Vinayakumar B | Vinayakumar B |
| [HDFS-7867](https://issues.apache.org/jira/browse/HDFS-7867) | Update action param from "start" to "prepare" in rolling upgrade javadoc |  Trivial | . | J.Andreina | J.Andreina |
| [HDFS-7501](https://issues.apache.org/jira/browse/HDFS-7501) | TransactionsSinceLastCheckpoint can be negative on SBNs |  Major | namenode | Harsh J | Gautam Gopalakrishnan |
| [HDFS-7261](https://issues.apache.org/jira/browse/HDFS-7261) | storageMap is accessed without synchronization in DatanodeDescriptor#updateHeartbeatState() |  Major | . | Ted Yu | Brahma Reddy Battula |
| [HDFS-6945](https://issues.apache.org/jira/browse/HDFS-6945) | BlockManager should remove a block from excessReplicateMap and decrement ExcessBlocks metric when the block is removed |  Critical | namenode | Akira AJISAKA | Akira AJISAKA |
| [HDFS-5356](https://issues.apache.org/jira/browse/HDFS-5356) | MiniDFSCluster shoud close all open FileSystems when shutdown() |  Critical | test | haosdent | Rakesh R |
| [HDFS-3325](https://issues.apache.org/jira/browse/HDFS-3325) | When configuring "dfs.namenode.safemode.threshold-pct" to a value greater or equal to 1 there is mismatch in the UI report |  Minor | . | J.Andreina | J.Andreina |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HDFS-6408](https://issues.apache.org/jira/browse/HDFS-6408) | Remove redundant definitions in log4j.properties |  Minor | test | Abhiraj Butala | Abhiraj Butala |
| [HDFS-6263](https://issues.apache.org/jira/browse/HDFS-6263) | Remove DRFA.MaxBackupIndex config from log4j.properties |  Minor | . | Akira AJISAKA | Abhiraj Butala |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HDFS-7854](https://issues.apache.org/jira/browse/HDFS-7854) | Separate class DataStreamer out of DFSOutputStream |  Major | hdfs-client | Li Bo | Li Bo |
| [HDFS-7713](https://issues.apache.org/jira/browse/HDFS-7713) | Implement mkdirs in the HDFS Web UI |  Major | . | Ravi Prakash | Ravi Prakash |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |

