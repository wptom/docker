# Docker configs
Tested docker configurations.

## XAMPP Configuration

- Download XAMPP image;

`docker pull tomsik68/xampp`

- Create instance of XAMPP where '/Sites/mysite' is physical location of your site; 

`docker run --name myXampp -p 41061:22 -p 41062:80 -d -v ~/Sites/mysite:/www tomsik68/xampp`

### URLs
- [XAMPP admin - http://localhost:41062/dashboard/](http://localhost:41062/dashboard/)
- [mysite - http://localhost:41062/www/](http://localhost:41062/www/)

### MySQL credentials: 
- username: root
- password is empty

More info about [XAMPP Docker image](https://hub.docker.com/r/tomsik68/xampp/)
