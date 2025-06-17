# static-website-ci-cd

Ejemplo que realizar auto CI/CD en AWS S3 sirviendo un sitio estatico.
Actualiza S3 cada que realiza push a la rama main


## Policies AWS

| Policy        |
|---------------|
| SamFullAccess |
|               |

# Politicas de Role

|                       |
|-----------------------|
| iam:AttachRolePolicy  |
| iam:DetachRolePolicy  |
| iam:CreateRole        |
| iam:TagRole           |
| iam:GetRole           |
| iam:DeleteRole        |
| iam:CreatePolicy      |
| iam:PutRolePolicy     |

## Variables 
### Secrets and Variables 
#### Actions
##### Repository Secrets

| Descripcion              | Valor                 |
|--------------------------|-----------------------|
| AWS_ACCESS_KEY_ID        | AWS Access Key ID     |
| AWS_SECRET_ACCESS_KEY    | AWS Secret Access Key |
| AWS_REGION               | AWS Región            |
| S3_BUCKET                | Nombre del Bucket     |
| STACK_NAME               | Nombre del Stack      |



```
git push origin main
```

```
Endpoint. http://<bucket>.s3-website.<region>.amazonaws.com/
```
