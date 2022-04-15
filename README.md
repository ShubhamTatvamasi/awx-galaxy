# awx-galaxy

Install dependant collections:
```bash
ansible-galaxy collection install shubhamtatvamasi.magma
```

Install AWX:
```bash
ansible-playbook deploy-awx.yml
```
> It takes 10 minutes to start after deployment is done.

ID: `admin`, get password:
```bash
kubectl get secret awx-admin-password -o jsonpath='{.data.password}' | base64 -d ; echo
```
