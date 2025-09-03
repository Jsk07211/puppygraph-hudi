Components of the project:
- Storage: MinIO/S3 (object store for Hudi data)
- Table format & writes: Apache Hudi (Spark writes)
- Catalog: Hive Metastore (backed by Postgres)
- Execution engine: Spark
- Graph engine: PuppyGraph

To populate the database (but it's not working):
```
docker compose exec spark /opt/spark/bin/spark-sql -f /init.sql
```