FROM debian:stable-slim

RUN apt-get update -y
RUN apt-get install -y curl telnet htop mtr wget vim
RUN curl -s https://packagecloud.io/install/repositories/ookla/speedtest-cli/script.deb.sh | bash
RUN apt-get install -y speedtest nginx ssh
COPY .ssh/ /root/.ssh

CMD ["nginx", "-g", "daemon off;"]