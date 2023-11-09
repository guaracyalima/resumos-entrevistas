# Trabalhando com namespaces

## Remover todos os pods em um namespace

```bash
kubectl delete pods --all -n [namespace]
```

## Remover namespace
```bash
kubectl delete namespace [your-namespace]
```

## Detalhes de um pod por namespace

```bash
kubectl describe pod {pod-name} -n {namespace-name}
```
