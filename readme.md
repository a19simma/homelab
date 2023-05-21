![Grafana](https://argo.simonmalm.com/api/badge?name=monitoring&revision=true) Grafana

![Cert-Manager](https://argo.simonmalm.com/api/badge?name=cert-manager&revision=true) Cert-Manager

![Traefik](https://argo.simonmalm.com/api/badge?name=traefik&revision=true) Traefik

![Vault](https://argo.simonmalm.com/api/badge?name=vault&revision=true) HashiCorp Vault

![Volsync](https://argo.simonmalm.com/api/badge?name=volsync&revision=true) Volsync

![Nextcloud](https://argo.simonmalm.com/api/badge?name=nextcloud&revision=true) Nextcloud

![Jellyfin](https://argo.simonmalm.com/api/badge?name=media-library&revision=true) Jellyfin

![Metallb](https://argo.simonmalm.com/api/badge?name=metallb&revision=true) Metallb

![Harbor](https://argo.simonmalm.com/api/badge?name=harbor&revision=true) Harbor

![Drone](https://argo.simonmalm.com/api/badge?name=drone&revision=true) Drone


# Cluster configuration using Argo-CD

wget https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.19.4/kubeseal-0.19.4-linux-amd64.tar.gz
tar -xvzf kubeseal-0.19.4-linux-amd64.tar.gz kubeseal
sudo install -m 755 kubeseal /usr/local/bin/kubeseal


# Passthrough disk to proxmox vm
`lshw -class disk -class storage`
`ls -l /dev/disk/by-id | grep <serial>`
`qm set 102 -scsi2 /dev/disk/by-id/ata-xxxxxxxxxxxxxxx`
