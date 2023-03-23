![Grafana](https://argo.simonmalm.com/api/badge?name=monitoring)
![Cert-Manager](https://argo.simonmalm.com/api/badge?name=cert-manager)
![Traefik](https://argo.simonmalm.com/api/badge?name=traefik)
![Rook-Ceph](https://argo.simonmalm.com/api/badge?name=rook-ceph)
![Volsync](https://argo.simonmalm.com/api/badge?name=volsync)
![Nextcloud](https://argo.simonmalm.com/api/badge?name=nextcloud)
![Jellyfin](https://argo.simonmalm.com/api/badge?name=media-library)
![Metallb](https://argo.simonmalm.com/api/badge?name=metallb)
![Harbor](https://argo.simonmalm.com/api/badge?name=harbor)
![Drone](https://argo.simonmalm.com/api/badge?name=drone)
![Gitea](https://argo.simonmalm.com/api/badge?name=gitea)

# Cluster configuration using Argo-CD

wget https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.19.4/kubeseal-0.19.4-linux-amd64.tar.gz
tar -xvzf kubeseal-0.19.4-linux-amd64.tar.gz kubeseal
sudo install -m 755 kubeseal /usr/local/bin/kubeseal


# Passthrough disk to proxmox vm
`lshw -class disk -class storage`
`ls -l /dev/disk/by-id | grep <serial>`
`qm set 102 -scsi2 /dev/disk/by-id/ata-xxxxxxxxxxxxxxx`