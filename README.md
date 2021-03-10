## Counter
This is easy word and characters counter!
[Demo](https://xhyrom.github.io/Counter/)

### Deploy on web-server or shared web-hosting
Copy all files from this repository to your web-server's root folder.

### Deploy with Docker
1. Install Docker
2. Run container -image:chobotnice/counter
                 -port:map port 80 inside container into some port of outside you server
Additonaly map   -volume: /usr/local/apache2/htdocs/ inside of container into some folder on your server

  Dcoker run command example
  > docker run --name counter -v /home/user/counterdata:/usr/local/apache2/htdocs/ -p 80:80 chobotnice/counter
