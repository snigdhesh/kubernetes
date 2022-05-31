
Make sure you follow these steps, else you may face issue while running worker-pod.yml

**Note:**   
Use `image: postgres:9.4` on `postgres-pod.yml`

**Sequence of object creations on cluster:**
- voting-app-pod.yaml
- voting-app-service.yaml
- redis-pod.yaml
- redis-service.yaml
- postgres-pod.yaml
- postgres-service.yaml
- worker-app-pod.yaml
- result-app-pod.yaml
- result-app-service.yaml



