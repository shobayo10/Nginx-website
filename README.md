# Nginx-website

REQUIREMENT 

step 1
Start an instance of NGINX in Docker with included Directory "website"

step 2 
Name container "website"

step 3 
website should be accessible at http://localhost:8080

step 4 
Map outside website dir $PWD/website: to inside the container > /usr/share/nginx/html to container.

SOLUTION
 docker run --name website -v "$PWD/website:/usr/share/nginx/html" -p 8080:80 --rm nginx

 Open new browser and input http://localhost:8080 to view website 
