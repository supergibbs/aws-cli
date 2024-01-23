FROM public.ecr.aws/amazonlinux/amazonlinux:2

RUN yum install -y unzip jq findutils \
    && yum clean all \
    && rm -rf /var/cache/yum

#Install awscli v2
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
    && unzip awscliv2.zip \
    && ./aws/install --bin-dir /usr/local/bin --install-dir /usr/local/aws-cli --update \
    && rm awscliv2.zip \
    && rm -rf ./aws
