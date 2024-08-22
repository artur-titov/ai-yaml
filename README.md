# YAML manifests crerated with AI 




| NAME                    | PROMPT      | DESCRIPTION | EXAMPLE |
| ----------------------- | ----------- | ----------- | ------- |
| app.yaml                | Create a pod for demo app with gcr.io/k8s-k3s/demo:v1.0.0 image, label demo and port 8080. This Pod must be cpu (1) and memory (2Gi) limited.| Basic Pod yaml | [Raw yaml](https://raw.githubusercontent.com/artur-titov/ai-yaml/main/yaml/app.yaml) |
| app-livenessProbe.yaml  | Add liveness probe to /health path with 10 sec delay | Updated app.yaml | [Raw yaml](https://raw.githubusercontent.com/artur-titov/ai-yaml/main/yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml | Add readiness probe to /ready path with 5 sec period | Updated app.yaml | [Raw yaml](https://raw.githubusercontent.com/artur-titov/ai-yaml/main/yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml   | Add data volume from host machine (/var/lib/app) and mount into container to /data path | Updated app.yaml | [Raw yaml](https://raw.githubusercontent.com/artur-titov/ai-yaml/main/yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml        | Create a cronjob yaml that will run the "echo "hello world"" command in the demo-app container every 5 minutes constantly | Cronjob yaml | [Raw yaml](https://raw.githubusercontent.com/artur-titov/ai-yaml/main/yaml/app-cronjob.yaml) |
| app-job.yaml            | |||
| app-multicontainer.yaml | Create a multi container pod for demo app with nginx image in first container and redis in second. Add label demo. This Pod must be cpu (2) and memory (2Gi) limited. Connect /usr/app/ directory to /var/www/html directory in nginx container. | Multi container Pod | [Raw yaml](https://raw.githubusercontent.com/artur-titov/ai-yaml/main/yaml/app-multicontainer.yaml) |
| app-resources.yaml      | |||
| app-secret-env.yaml     | |||