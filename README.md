# BigSchool
# file: inventories.hosts

storage-ceph01 ansible_ssh_host=172.20.160.201
storage-ceph02 ansible_ssh_host=172.20.160.202
storage-ceph03 ansible_ssh_host=172.20.160.203
storage-ceph04 ansible_ssh_host=172.20.160.204
storage-ceph05 ansible_ssh_host=172.20.160.205

[storage-ceph_engine]
storage-ceph01
storage-ceph02
storage-ceph03
storage-ceph04
storage-ceph05


[mons]
storage-ceph01
storage-ceph02
storage-ceph03
storage-ceph04
storage-ceph05

[osds]
storage-ceph01
storage-ceph02
storage-ceph03
storage-ceph04
storage-ceph05

[mgrs]
storage-ceph01
storage-ceph02
storage-ceph03
storage-ceph04
storage-ceph05

[monitoring]
storage-ceph01
storage-ceph02
storage-ceph03

[mdss]
storage-ceph01

[all:vars]
ansible_connection=ssh
ansible_user=root
