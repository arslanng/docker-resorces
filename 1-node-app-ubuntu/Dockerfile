FROM ubuntu:18.04
RUN apt-get update
RUN apt-get install curl -y
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get install nodejs -y
COPY . /opt/node-app/
ENV channel=kablosuzkedi
# Yukarıdaki kısım imageden container oluşturmak için
# aşağıdaki kısım oluşan containerın çalışma anında çalışacak kısım.
# CMD [ "node", "/opt/node-app/index.js" ]
WORKDIR /opt/node-app/
CMD [ "node", "index.js" ]