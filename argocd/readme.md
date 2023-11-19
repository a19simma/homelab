# Add and Install the argocd helm chart
`helm repo add argo https://argoproj.github.io/argo-helm`
`helm upgrade argocd argo/argo-cd -n argocd`


## Argocd setup
Apply all the k8s manifests in the argocd folder.
Install the charts with the value files in the chart subdir