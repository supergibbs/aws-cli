FROM public.ecr.aws/amazonlinux/amazonlinux:2023

RUN dnf install -y awscli jq findutils gzip \
    && dnf clean all \
    && rm -rf /var/cache/yum
