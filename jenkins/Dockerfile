FROM jenkins:2.60.3 

USER root

RUN apt-key adv --keyserver keyserver.ubuntu.com --recv DF7D54CBE56151BF && \
    ( echo "deb http://repos.mesosphere.com/debian stretch main" | \
    tee /etc/apt/sources.list.d/mesosphere.list ) && \
    apt-get -y update && \
    apt-get -y install systemd mesos=1.3.*

RUN /usr/local/bin/install-plugins.sh \
    ace-editor:1.1	\
    ant:1.7	\
    antisamy-markup-formatter:1.5	\
    authentication-tokens:1.3	\
    blueocean-autofavorite:1.0.0	\
    blueocean-bitbucket-pipeline:1.2.0	\
    blueocean-commons:1.2.0	\
    blueocean-config:1.2.0	\
    blueocean-dashboard:1.2.0	\
    blueocean-display-url:2.1.0	\
    blueocean-events:1.2.0	\
    blueocean-git-pipeline:1.2.0	\
    blueocean-github-pipeline:1.2.0	\
    blueocean-i18n:1.2.0	\
    blueocean-jwt:1.2.0	\
    blueocean-personalization:1.2.0	\
    blueocean-pipeline-api-impl:1.2.0	\
    blueocean-pipeline-editor:1.2.0	\
    blueocean-pipeline-scm-api:1.2.0	\
    blueocean-rest-impl:1.2.0	\
    blueocean-rest:1.2.0	\
    blueocean-web:1.2.0	\
    blueocean:1.2.0	\
    bouncycastle-api:2.16.2	\
    branch-api:2.0.11	\
    build-timeout:1.18	\
    cloudbees-bitbucket-branch-source:2.2.3	\
    cloudbees-folder:6.1.2	\
    credentials-binding:1.13	\
    credentials:2.1.14	\
    display-url-api:2.0	\
    docker-commons:1.8	\
    docker-workflow:1.12	\
    durable-task:1.14	\
    email-ext:2.58	\
    external-monitor-job:1.7	\
    favorite:2.3.0	\
    git-client:2.5.0	\
    git-server:1.7	\
    git:3.5.1	\
    github-api:1.86	\
    github-branch-source:2.2.3	\
    github:1.28.0	\
    gradle:1.27.1	\
    handlebars:1.1.1	\
    htmlpublisher:1.14	\
    icon-shim:2.0.3	\
    jackson2-api:2.7.3	\
    javadoc:1.4	\
    jira:2.4.2	\
    jquery-detached:1.2.1	\
    junit:1.21	\
    ldap:1.16	\
    mailer:1.20	\
    mapdb-api:1.0.9.0	\
    matrix-auth:1.7	\
    matrix-project:1.11	\
    mercurial:2.1	\
    mesos:0.15.0	\
    metrics:3.1.2.10	\
    momentjs:1.1.1	\
    pam-auth:1.3	\
    pipeline-build-step:2.5.1	\
    pipeline-github-lib:1.0	\
    pipeline-graph-analysis:1.5	\
    pipeline-input-step:2.8	\
    pipeline-milestone-step:1.3.1	\
    pipeline-model-api:1.1.9	\
    pipeline-model-declarative-agent:1.1.1	\
    pipeline-model-definition:1.1.9	\
    pipeline-model-extensions:1.1.9	\
    pipeline-rest-api:2.9	\
    pipeline-stage-step:2.2	\
    pipeline-stage-tags-metadata:1.1.9	\
    pipeline-stage-view:2.9	\
    plain-credentials:1.4	\
    prometheus:1.1.0	\
    pubsub-light:1.12	\
    resource-disposer:0.7	\
    scm-api:2.2.1	\
    script-security:1.33	\
    skip-certificate-check:1.0	\
    sse-gateway:1.15	\
    ssh-credentials:1.13	\
    ssh-slaves:1.21	\
    structs:1.10	\
    subversion:2.9	\
    timestamper:1.8.8	\
    token-macro:2.3	\
    variant:1.1	\
    windows-slaves:1.3.1	\
    workflow-aggregator:2.5	\
    workflow-api:2.20	\
    workflow-basic-steps:2.6	\
    workflow-cps-global-lib:2.8	\
    workflow-cps:2.39	\
    workflow-durable-task-step:2.15	\
    workflow-job:2.12.2	\
    workflow-multibranch:2.16	\
    workflow-scm-step:2.6	\
    workflow-step-api:2.12	\
    workflow-support:2.14	\
    ws-cleanup:0.34	

# USER jenkins
