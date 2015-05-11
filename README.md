The purpose of this project is to install an Openstack Enviroment
The objective of this is to:
Install the controllers in a highly available configuration
  - controller nodes are to have openstack services installed, in accordance with https://access.redhat.com/site/documentation/en-US/Red_Hat_Enterprise_Linux_OpenStack_Platform/6/html/Installer_and_Foreman_Guide/index.html
  - setting up pacemaker and corosync and haproxy to allow for ha services according to http://docs.openstack.org/high-availability-guide/content/ch-intro.html
  - configure glance swift and cinder to use ceph for backend storage -
Install a ceph cluster for volume and image storage
  - setup cluster with 3 monitors and at least 3 osd nodes
  - setup radosgw with keystone auth
Install compute nodes
  - setup nova-compute with rbd support for volumes
  - setup ovs-agent

To subscribe using subscription-manager pass the following 3 varables via cli
  - rhn-user
  - rhn-pass
  - pool
