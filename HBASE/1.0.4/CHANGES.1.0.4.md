
<!---
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
-->
# Apache HBase Changelog

## Release 1.0.4 - Unreleased (as of 2016-03-01)

### INCOMPATIBLE CHANGES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPORTANT ISSUES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### NEW FEATURES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### IMPROVEMENTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HBASE-15129](https://issues.apache.org/jira/browse/HBASE-15129) | Set default value for hbase.fs.tmp.dir rather than fully depend on hbase-default.xml |  Major | mapreduce | Yu Li | Yu Li |


### BUG FIXES:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HBASE-15274](https://issues.apache.org/jira/browse/HBASE-15274) | ClientSideRegionScanner's reaction to Scan#setBatch is not consistent between HBase versions |  Minor | . | Youngjoon Kim | Youngjoon Kim |
| [HBASE-15252](https://issues.apache.org/jira/browse/HBASE-15252) | Data loss when replaying wal if HDFS timeout |  Blocker | wal | Duo Zhang | Duo Zhang |
| [HBASE-15218](https://issues.apache.org/jira/browse/HBASE-15218) | On RS crash and replay of WAL, loosing all Tags in Cells |  Blocker | Recovery, regionserver, security | Anoop Sam John | Anoop Sam John |
| [HBASE-15214](https://issues.apache.org/jira/browse/HBASE-15214) | Valid mutate Ops fail with RPC Codec in use and region moves across |  Critical | . | Anoop Sam John | Anoop Sam John |
| [HBASE-15200](https://issues.apache.org/jira/browse/HBASE-15200) | ZooKeeper znode ACL checks should only compare the shortname |  Minor | security | Andrew Purtell | Andrew Purtell |
| [HBASE-15198](https://issues.apache.org/jira/browse/HBASE-15198) | RPC client not using Codec and CellBlock for puts by default |  Critical | . | Anoop Sam John | Anoop Sam John |
| [HBASE-15152](https://issues.apache.org/jira/browse/HBASE-15152) | Automatically include prefix-tree module in MR jobs if present |  Major | mapreduce | Jonathan Hsieh | Jonathan Hsieh |
| [HBASE-15150](https://issues.apache.org/jira/browse/HBASE-15150) | Fix TestDurablity in branch-1.1 |  Major | test | Yu Li | Yu Li |
| [HBASE-15147](https://issues.apache.org/jira/browse/HBASE-15147) | Shell should use Admin.listTableNames() instead of Admin.listTables() |  Major | . | Enis Soztutar | Enis Soztutar |
| [HBASE-15122](https://issues.apache.org/jira/browse/HBASE-15122) | Servlets generate XSS\_REQUEST\_PARAMETER\_TO\_SERVLET\_WRITER findbugs warnings |  Critical | . | stack | Samir Ahmic |
| [HBASE-15019](https://issues.apache.org/jira/browse/HBASE-15019) | Replication stuck when HDFS is restarted |  Major | Replication, wal | Matteo Bertozzi | Matteo Bertozzi |
| [HBASE-14460](https://issues.apache.org/jira/browse/HBASE-14460) | [Perf Regression] Merge of MVCC and SequenceId (HBASE-8763) slowed Increments, CheckAndPuts, batch operations |  Critical | Performance | stack | stack |


### TESTS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


### SUB-TASKS:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |
| [HBASE-15224](https://issues.apache.org/jira/browse/HBASE-15224) | Undo  "hbase.increment.fast.but.narrow.consistency" option; it is not necessary since HBASE-15213 |  Major | Performance | stack | stack |
| [HBASE-15213](https://issues.apache.org/jira/browse/HBASE-15213) | Fix increment performance regression caused by HBASE-8763 on branch-1.0 |  Major | Performance | Junegunn Choi | Junegunn Choi |
| [HBASE-15157](https://issues.apache.org/jira/browse/HBASE-15157) | Add \*PerformanceTest for Append, CheckAnd\* |  Major | Performance, test | stack | stack |
| [HBASE-15153](https://issues.apache.org/jira/browse/HBASE-15153) | Apply checkFamilies addendum on increment to 1.1 and 1.0 |  Major | Performance | stack | stack |


### OTHER:

| JIRA | Summary | Priority | Component | Reporter | Contributor |
|:---- |:---- | :--- |:---- |:---- |:---- |


