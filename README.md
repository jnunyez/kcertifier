# oranDetect 

A simple tool to scan useful info regarding HW and SW releases in multiple OCP clusters devoted to O-RAN workloads. The usual suspects to scan and certify are SRIOV operators, kernel drivers, NIC firmware, BIOS version, 5G-acccelerators cards....

## Quickstart

1) Download the repo in a node with openshift CLI installed and ssh access by private key to all the nodes in the cluster under scan
2) Check that KUBECONFIG environment variable is already initiated to the target cluster (if it does `oc get nodes` should return something).
3) Execute the script with exactly one argument:
      ```
      ./scanner/oranDetect <SSH_ABSOLUTE_KEY_PATH>
      ```
SSH_ABSOLUTE_KEY_PATH is the absolute private ssh key path to access by ssh to all the nodes in the cluster
