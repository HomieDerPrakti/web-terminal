FROM ubuntu:latest

ADD https://github.com/tsl0922/ttyd/releases/download/1.7.3/ttyd.x86_64 /usr/local/bin/ttyd
RUN chmod +x /usr/local/bin/ttyd

RUN apt-get update && apt-get install -y \
	neofetch
RUN echo "neofetch" >> /root/.bashrc

EXPOSE 7681

CMD ["ttyd", "bash"]
