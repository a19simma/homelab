```
echo -n SECRET-PASSWORD | kubeseal --controller-name sealed-secrets --controller-namespace sealed-secrets --raw --namespace traefik --name traefik-dashboard-auth
```