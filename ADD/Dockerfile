FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.github.com/durgaprasadkothapalli/vpc-module-test/blob/main/output.tf /usr/share/nginx/html/index.html
RUN chmod +x /usr/share/nginx/index.html
ADD sample-1.tar /tmp/
CMD ["nginx","-g", "daemon off;"]
