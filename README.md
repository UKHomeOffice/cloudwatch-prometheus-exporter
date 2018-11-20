Prometheus Exporter for S3, API Gateway and Cloudwatch Events and Lambda Cloudwatch Metrics
=====

## Usage
* Run and mount the config passing your AWS creds
```
$ docker run -d \
             -e AWS_ACCESS_KEY_ID='' \
             -e AWS_SECRET_ACCESS_KEY='' \
             -p 9106:9106 \ 
             -v $(pwd)/config.yml:/config/config.yml prom/cloudwatch-exporter
$ curl localhost:9106/metrics
```
## TODO
* Create Kubernetes deployment/configmap resource YAML
* Enabled automated build to an image registry
