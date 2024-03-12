FROM xswitch.tencentcloudcr.com/xswitch/xswitch:bookworm as xswitch-build-bookworm
LABEL maintainer="Seven Du <dujinfang@x-y-t.cn>"
SHELL ["/bin/bash", "-c"]
RUN echo "deb http://apt.postgresql.org/pub/repos/apt bookworm-pgdg main" > /etc/apt/sources.list.d/pgdg.list
RUN wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | apt-key add -
RUN apt-get update && apt-get install -y postgresql-client-15
