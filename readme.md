# ruby libhdfs client

### requirements
  - ruby    (1.9.2 <=)
  - java    (1.6 <=)
  - libhdfs (2.x)

### installation
```
gem install ruby-hdfs-cdh4
```

this gem provides defaults for installation on machines using cdh4 and the hadoop-libhdfs cloudera package, but the following enviorment variables are available for configuration.

  - HADOOP_ENV
  - JAVA_HOME
  - JAVA_LIB

### usage
to setup your classpath on chd4 machines require `hdfs/classpath`, or see [classpath.rb](https://github.com/dallasmarlow/ruby-hdfs-cdh4/blob/master/lib/hdfs/classpath.rb) as an example.

```ruby
require 'hdfs/classpath'

dfs = Hadoop::DFS::FileSystem.new 'namenode.domain.tld', 8020
```