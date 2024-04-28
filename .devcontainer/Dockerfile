# [Choice] Ubuntu version (use jammy on local arm64/Apple Silicon): jammy, focal
FROM ubuntu:18.04

LABEL dev.containers.features="common"

# [Optional] Uncomment this section to install additional OS packages.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends htop

# - sudo apt-get update
# - sudo apt-get install -y libssl-dev libzookeeper-mt-dev protobuf-compiler libprotobuf-dev libboost-all-dev openjdk-8-jdk cmake
# - wget http://launchpadlibrarian.net/57653337/doxygen_1.7.1-2_amd64.deb
# - sudo dpkg -i doxygen_1.7.1-2_amd64.deb
