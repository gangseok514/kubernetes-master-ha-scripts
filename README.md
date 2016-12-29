# kubernetes-master-ha-scripts

This is patch for k8s master high availability in AWS provider. It customizes the shell scripts related kube-up.

You just copy and overwrite these files to kubernetes then you can make multi-master.

This patch is based on k8s v1.4.1

## Usage : Examples

    export KUBERNETES_PROVIDER=aws
    export KUBE_AWS_ZONE=us-west-1b
    export NUM_NODES=3
    export MASTER_SIZE=m3.large
    export NODE_SIZE=m3.large
    export AWS_S3_REGION=us-west-1
    export AWS_S3_BUCKET=k8s-ha
    export KUBE_AWS_INSTANCE_PREFIX=k8s-ha

    export ENABLE_MASTER_HA=true
    export NUM_MASTERS=3
