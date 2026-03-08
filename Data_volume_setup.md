    - lvremove /dev/pve/data

    - vgdisplay pve

    - lvcreate -l 100%FREE -n mydata pve

    - vgdisplay pve

    - mkfs.ext4 /dev/pve/mydata

    - mkdir /mnt/mydata

    - mount /dev/pve/mydata /mnt/mydata

    - df

    - vi /etc/fstab → /dev/pve/mydata  /mnt/mydata  ext4  defaults  0 2
