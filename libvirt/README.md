# enp7s0
virsh attach-interface --domain worker4 --type network --source wan --model virtio --config --live
virsh attach-interface --domain worker6 --type network --source wan --model virtio --config --live

# enp8s0
virsh attach-interface --domain worker4 --type network --source lan-r1 --model virtio --config --live
virsh attach-interface --domain worker6 --type network --source lan-r2 --model virtio --config --live