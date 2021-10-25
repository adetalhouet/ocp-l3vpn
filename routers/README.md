mkisofs -l -o r1/r1_config.iso r1/iosxe_config.txt
virtctl image-upload dv r1-config --access-mode ReadWriteMany --block-volume --storage-class=ocs-storagecluster-ceph-rbd --size=500Mi --image-path=./r1/r1_config.iso

mkisofs -l -o r2/r2_config.iso r2/iosxe_config.txt
virtctl image-upload dv r2-config --access-mode ReadWriteMany --block-volume --storage-class=ocs-storagecluster-ceph-rbd --size=500Mi --image-path=./r2/r2_config.iso