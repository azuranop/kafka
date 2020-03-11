```
git clone https://github.com/confluentinc/schema-registry.git
```

```
$ git checkout v5.2.0
```

# Follow 

https://github.com/confluentinc/kafka-connect-hdfs/issues/311

$ git diff pom.xml
diff --git a/pom.xml b/pom.xml
index e4193012..b3d16d27 100644
--- a/pom.xml
+++ b/pom.xml
@@ -71,10 +71,17 @@
         <repository>
             <id>confluent</id>
             <name>Confluent</name>
-            <url>${confluent.maven.repo}</url>
+            <url>http://packages.confluent.io/maven/</url>
         </repository>
     </repositories>
 
+    <pluginRepositories>
+        <pluginRepository>
+            <id>confluent</id>
+            <name>Confluent</name>
+            <url>http://packages.confluent.io/maven/</url>
+        </pluginRepository>
+    </pluginRepositories>
     <dependencyManagement>
         <dependencies>
             <dependency>
