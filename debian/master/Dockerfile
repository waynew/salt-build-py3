FROM debian:9
RUN apt-get update && apt-get install -y curl
RUN curl -L https://bootstrap.saltstack.com -o install_salt.sh
RUN sh install_salt.sh -M -X
ADD orch/ /srv/salt/orch/
ADD states/ /srv/salt/
