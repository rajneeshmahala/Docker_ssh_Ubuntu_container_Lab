ssh enabled ubuntu container docker file for testing and R&D.
passwd : "redhat"
usr : "root"
req step : > docker bulid . -t sshUbuntu:v1
           > docker run -itd --name "name" -p hostport:22 sshUbuntu:v1
           >ssh >>> ssh -p hostport root@127.0.0.1
           > passwd
           
