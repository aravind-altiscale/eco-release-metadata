
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
# Apache Tez  0.8.0-alpha Release Notes

These release notes cover new developer and user-facing incompatibilities, important issues, features, and major improvements.


---

* [TEZ-2565](https://issues.apache.org/jira/browse/TEZ-2565) | *Major* | **Consider scanning unfinished tasks in VertexImpl::constructStatistics to reduce merge overhead**

constructStatistics() can be an overhead (scanning all tasks and merging stats) depending on the number of invocations to Vertex::getStatistics().  Consider scanning only unfinished tasks.


---

* [TEZ-2468](https://issues.apache.org/jira/browse/TEZ-2468) | *Major* | **Change master to build against Java 7**

**WARNING: No release note provided for this incompatible change.**


---

* [TEZ-2048](https://issues.apache.org/jira/browse/TEZ-2048) | *Blocker* | **Remove VertexManagerPluginContext.getTaskContainer()**

This should have been removed earlier. It exposes internal execution details that may not be safe to provide to user code.


