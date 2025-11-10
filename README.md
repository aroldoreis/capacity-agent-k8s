# Capacity Agent - GitOps Manifests

Repositório de manifestos Kubernetes gerenciados pelo Capacity Agent via GitOps.

## Estrutura

```
manifests/
  default/          # Deployments do namespace default
argocd/
  applications/     # ArgoCD Applications
```

## Fluxo GitOps

1. Bot cria PR com mudanças
2. Time revisa e aprova
3. Merge para main
4. ArgoCD sincroniza automaticamente
