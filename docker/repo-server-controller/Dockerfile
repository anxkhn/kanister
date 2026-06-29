FROM registry.access.redhat.com/ubi9/ubi-minimal:9.8@sha256:c5478a52c410e71c53839923c83a1480199a1e74ce5736fe3e3a5578dc399102

LABEL maintainer="Kanister maintainers<kanister.maintainers@veeam.com>"

RUN microdnf -y update openssl-libs

ADD repo-server-controller /repo-server-controller
ENTRYPOINT ["/repo-server-controller"]
