# my_aidecipher_manifest

## 구조
    root
    ├── {application}
    │   ├── base
    │   └── overlays
    ├── .gitignore
    └── README.md
---
## 시크릿 
```
[DockerHub Image Pull 을 위한 시크릿 생성]
kubectl create secret -n {네임스페이스} docker-registry dockerhub-secret \
    --docker-server=https://index.docker.io/v1/ \
    --docker-email={...} \
    --docker-username={...} \
    --docker-password={...}

kubectl get secret -n {네임스페이스} -o wide
kubectl get secret dockerhub-secret -n {네임스페이스} -o yaml
```
