FROM debian:stable
ENV shellrunner=.  

RUN apt-get update && apt-get install -y --force-yes apache2 &&\
apt-get install -y git &&\
apt-get install -y sudo

#ADD $shellrunner/temp.sh .
#RUN ./temp.sh
#RUN sudo cp -R ./projCert /var/www/html
RUN sudo cp -R ../website /var/www/html

RUN "ls" "/var/www"

#WORKDIR /var/www/html/projCert
RUN chmod +x . 
EXPOSE 80 443

#ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
