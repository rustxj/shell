# shell
shell class


#docker http3


docker run --name nginx -d -p 80:80 -p 443:443/tcp -p 443:443/udp -v /root/dev.crt:/etc/ssl/dev.crt -v /root/dev.key:/etc/ssl/dev.key -v /root/http3.conf:/etc/nginx/nginx.conf ranadeeppolavarapu/nginx-http3:latest

#docker 2022dev



docker run --name nginx -dt -p 80:80 -p 443:443/tcp -v /home/m3.conf:/etc/nginx/nginx.conf ranadeeppolavarapu/nginx-http3:latest


#
docker run -dt  --net=host --restart=always -e IMGPROXY_KEY=576514d6bcf572f3499e253a9fcf2e9849e9792eb87ecc8ee098 -e IMGPROXY_CONCURRENCY=9999 -e IMGPROXY_SALT=81a1babfddd75816dfa5195f9a61ce19226705297ac7 -e IMGPROXY_USER_AGENT="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.183 Safari/537.36" -e IMGPROXY_MAX_SRC_RESOLUTION=36 -e IMGPROXY_DOWNLOAD_TIMEOUT=30 -e IMGPROXY_WATERMARK_PATH=/root/dev.svg -v /etc/resolv.conf:/etc/resolv.conf -v /root/dev.svg:/root/dev.svg -e IMGPROXY_ENFORCE_WEBP=false -e IMGPROXY_ENABLE_WEBP_DETECTION=false -e  IMGPROXY_USE_ETAG=true -e IMGPROXY_CACHE_CONTROL_PASSTHROUGH=true -e IMGPROXY_TTL=99999999999999 darthsim/imgproxy:latest


docker run --name nginxs -dt --net=host --restart=always -v /root/cache.conf:/etc/nginx/nginx.conf -v /cache:/cache ranadeeppolavarapu/nginx-http3:latest
