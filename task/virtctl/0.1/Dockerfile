FROM registry.access.redhat.com/ubi8/ubi

RUN yum update -y && \
    yum install -y wget && \
    wget -O /usr/local/bin/virtctl https://github.com/kubevirt/kubevirt/releases/download/v0.32.0/virtctl-v0.32.0-linux-x86_64 && \
    chmod +x /usr/local/bin/virtctl && \
    yum clean all && \
    rm -rf /var/cache/yum

USER 1001

ENTRYPOINT ["/usr/local/bin/virtctl"]
