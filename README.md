docker run -p 80:80 -p 443:443 -v ./app.crt:/etc/nginx/certs/app1-test.com.crt -v ./app.key:/etc/nginx/certs/app1-test.com.key -v ./ca.crt:/etc/nginx/certs/ca.crt -v ./config/nginx.conf:/etc/nginx/nginx.conf --net=host nginx:latest 

be sure that set properly and meteor container has open port to localhost
APP_ROOT_URL="http://app1-test.com"
ROOT_URL="http://app1-test.com" 
