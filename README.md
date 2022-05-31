
Make sure you follow these steps, else you may face issue while running worker-pod.yml

**Note:**   
Use `image: postgres:9.4` on `postgres-pod.yml`

**Sequence of object creations on cluster (when no deloyments were created):**
- voting-app-pod.yaml
- voting-app-service.yaml
- redis-pod.yaml
- redis-service.yaml
- postgres-pod.yaml
- postgres-service.yaml
- worker-app-pod.yaml
- result-app-pod.yaml
- result-app-service.yaml


# While development

- First we created pods
- Then services
- Then deployments #Deployments are like wrappers around pod.  

**Sequence of object creations on cluster (when deloyments were created):**
- voting-app-deploy.yaml
- voting-app-service.yaml
- redis-deploy.yaml
- redis-service.yaml
- postgres-deploy.yaml
- postgres-service.yaml
- worker-app-deploy.yaml
- result-app-deploy.yaml
- result-app-service.yaml





