# shell
shell class


#docker http3
docker run --name nginx -d -p 80:80 -p 443:443/tcp -p 443:443/udp -v /root/dev.crt:/etc/ssl/dev.crt -v /root/dev.key:/etc/ssl/dev.key -v /root/http3.conf:/etc/nginx/nginx.conf ranadeeppolavarapu/nginx-http3:latest

#docker 2022dev
docker run --name nginx -dt -p 80:80 -p 443:443/tcp -v /root/m3.conf:/etc/nginx/nginx.conf ranadeeppolavarapu/nginx-http3:latest