FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/Sameer-Sarrainodu/Ansible-Roboshop/refs/heads/main/payment.ini /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
ADD sample-1.tar /tmp/
CMD [ "nginx", "-g", "daemon off;" ]