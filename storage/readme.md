# Useful notes on disk management

## Passthrough disk to proxmox vm
`lshw -class disk -class storage`
`ls -l /dev/disk/by-id | grep <serial>`
`qm set 102 -scsi2 /dev/disk/by-id/ata-xxxxxxxxxxxxxxx`
