![Grafana](https://argo.simonmalm.com/api/badge?name=monitoring) Grafana

![Cert-Manager](https://argo.simonmalm.com/api/badge?name=cert-manager) Cert-Manager

![Traefik](https://argo.simonmalm.com/api/badge?name=traefik) Traefik

![Rook-Ceph](https://argo.simonmalm.com/api/badge?name=rook-ceph) Rook-Ceph

![Vault](https://argo.simonmalm.com/api/badge?name=vault) HashiCorp Vault

![Volsync](https://argo.simonmalm.com/api/badge?name=volsync) Volsync

![Nextcloud](https://argo.simonmalm.com/api/badge?name=nextcloud) Nextcloud

![Jellyfin](https://argo.simonmalm.com/api/badge?name=media-library) Jellyfin

![Metallb](https://argo.simonmalm.com/api/badge?name=metallb) Metallb

![Harbor](https://argo.simonmalm.com/api/badge?name=harbor) Harbor

![Drone](https://argo.simonmalm.com/api/badge?name=drone) Drone

![Gitea](https://argo.simonmalm.com/api/badge?name=gitea) Gitea


# Cluster configuration using Argo-CD

wget https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.19.4/kubeseal-0.19.4-linux-amd64.tar.gz
tar -xvzf kubeseal-0.19.4-linux-amd64.tar.gz kubeseal
sudo install -m 755 kubeseal /usr/local/bin/kubeseal


# Passthrough disk to proxmox vm
`lshw -class disk -class storage`
`ls -l /dev/disk/by-id | grep <serial>`
`qm set 102 -scsi2 /dev/disk/by-id/ata-xxxxxxxxxxxxxxx`