# Hadoop  2.1.1-beta Release Notes

These release notes cover new developer and user-facing incompatibilities, features, and major improvements.


---

* [HADOOP-9944](https://issues.apache.org/jira/browse/HADOOP-9944) | *Blocker* | **RpcRequestHeaderProto defines callId as uint32 while ipc.Client.CONNECTION\_CONTEXT\_CALL\_ID is signed (-3)**

**WARNING: No release note provided for this incompatible change.**


---

* [HDFS-5118](https://issues.apache.org/jira/browse/HDFS-5118) | *Major* | **Provide testing support for DFSClient to drop RPC responses**

Used for testing when NameNode HA is enabled. Users can use a new configuration property "dfs.client.test.drop.namenode.response.number" to specify the number of responses that DFSClient will drop in each RPC call. This feature can help testing functionalities such as NameNode retry cache.


---

* [YARN-1170](https://issues.apache.org/jira/browse/YARN-1170) | *Blocker* | **yarn proto definitions should specify package as 'hadoop.yarn'**

**WARNING: No release note provided for this incompatible change.**


---

* [YARN-707](https://issues.apache.org/jira/browse/YARN-707) | *Blocker* | **Add user info in the YARN ClientToken**

**WARNING: No release note provided for this incompatible change.**


