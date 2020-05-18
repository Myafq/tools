FROM alpine:3.11.6
ARG kustomize_version=3.5.5
ARG kubectl_version=v1.18.2
RUN wget -O /tmp/kustomize.tar.gz https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize/v${kustomize_version}/kustomize_v${kustomize_version}_linux_amd64.tar.gz &&\
    wget -O /usr/local/bin/kubectl https://storage.googleapis.com/kubernetes-release/release/${kubectl_version}/bin/linux/amd64/kubectl &&\
    cd /tmp && tar xf kustomize.tar.gz && mv /tmp/kustomize /usr/local/bin/ &&\
    chmod +x /usr/local/bin/*

