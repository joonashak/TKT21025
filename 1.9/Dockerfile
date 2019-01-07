FROM ubuntu:16.04

# Java
RUN apt-get update
RUN apt-get install -y openjdk-8-jre-headless

# Leiningen
RUN apt-get install -y wget
RUN wget https://raw.githubusercontent.com/technomancy/leiningen/stable/bin/lein
RUN chmod a+x lein
RUN mv lein /bin
RUN lein

# Port for nREPL
EXPOSE 33111

CMD ["/bin/bash"]
