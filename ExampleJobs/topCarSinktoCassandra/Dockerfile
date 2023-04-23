#licensed to the Apache Software Foundation (ASF) under one
#  or more contributor license agreements.  See the NOTICE file
#  distributed with this work for additional information
#  regarding copyright ownership.  The ASF licenses this file
#  to you under the Apache License, Version 2.0 (the
#  "License"); you may not use this file except in compliance
#  with the License.  You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
#  Unless required by applicable law or agreed to in writing, software
#  distributed under the License is distributed on an "AS IS" BASIS,
#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#  See the License for the specific language governing permissions and
# limitations under the License.
################################################################################

FROM harbor-repo.vmware.com/flinksolution/apache/flink:latest

RUN curl -k -L -o /opt/flink/lib/flink-connector-cassandra-1.16.1.jar  https://146.75.40.209/maven2/org/apache/flink/flink-connector-cassandra_2.12/1.16.1/flink-connector-cassandra_2.12-1.16.1.jar
RUN mkdir /opt/flink/usrlib
ADD target/TopSpeedWindowing.jar /opt/flink/usrlib/TopWindowingCassandra.jar
RUN chown -R flink:flink /opt/flink/usrlib
