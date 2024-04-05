# om_flyway_poc


a.b.c
a - source_type [1. Oracle, 2. FlatFiles]
b - Script Number
c - Version
            set JAVA_ARGS=--add-opens=java.base/java.nio=ALL-UNNAMED


            flyway -outOfOrder=true -url='jdbc:snowflake://https://lh29894.ap-southeast-1.snowflakecomputing.com' -user='svc' -password='Samplepassword#9' -initSql="USE ROLE ACCOUNTADMIN;USE WAREHOUSE COMPUTE_WH;USE DATABASE FLYWAY_POC;USE SCHEMA UTIL;" -locations=filesystem:sources info
