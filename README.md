# kind-tekton-argocd

Demo to deploy a local kind cluster with tekton and argocd

## Prepare WSL

```bash
pip install ansible ansible-lint kubernetes
```

## Run Playbook

```bash
ansible-playbook kind.yml
```

## Port-Forward Argo and Tekton

```bash
kubectl port-forward svc/argocd-server 8443:443 -n argocd
```
