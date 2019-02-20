# sample-confd-config
A sample confd config for use with
[s2i-confd](https://github.com/atgreen/s2i-confd.git) on
[OpenShift](https://www.openshift.com).

This example watches an IP value stored in etcd, and invokes an
[Ansible Tower](https://www.ansible.com/products/tower) job template
whenever it changes.

This is the "source" for the confd s2i builder.  Use it as you would
any s2i build in [OpenShift](https://www.openshift.com), or build your
container image manually like so:

    $ s2i build https://github.com/atgreen/sample-confd-config.git atgreen/s2i-confd dyndns-trigger


The ansible playbook is here:
https://github.com/atgreen/s2i-confd-dyndns-playbook-example.git

s2i-confd is here: https://github.com/atgreen/s2i-confd.git



