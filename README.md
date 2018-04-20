# Jmeter-benchmark

Jmeter-benchmark is a docker image containing a tuned jmeter.

### Run a basic benchmark

```bash
  TEST_PLAN=test-plan.jmx \
  USER=centos THREADS="300" \
  INJECTOR_HOST="injector_host" \
  DURATION=300 \
  TARGET_HOST="target_host" \
  TARGET_HOST_HEADER="target_host" \
  PROTOCOL="http" \
  TARGET_PORT="8081" \
  RPS=500  \
  TARGET_PATH="/some-request?user_key=USER_KEY" make run_benchmark
```
