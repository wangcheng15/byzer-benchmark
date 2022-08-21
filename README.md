# byzer-benchmark

## Running tpc-ds benchmark
1. edit run-benchmark.sh, replace classpath with your real path
2. run run-benchmark.sh , example:
```shell
./run-benchmark.sh --tpcdsDataDir s3a://byzer-bm/ \
--reportDir /tmp \
--engineUrl http://localhost:9004 \
--defaultPathPrefix /tmp/byzer-lang \
--failureCountThreshold 99 \
--useJuiceFS false \
--scaleFactor 1gb \
--format parquet
```