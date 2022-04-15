# awx-galaxy

Install AWX:
```bash
ansible-playbook deploy-awx.yml
```

ID: `admin`, get password:
```bash
kubectl get secret awx-admin-password -o jsonpath='{.data.password}' | base64 -d ; echo
```
