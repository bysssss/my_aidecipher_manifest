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
1) DockerHub Image Pull
kubectl create secret -n {네임스페이스} docker-registry dockerhub-secret \
    --docker-server=https://index.docker.io/v1/ \
    --docker-email={...} \
    --docker-username={...} \
    --docker-password={...}
```
