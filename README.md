# recommendations-proxy

Proxy server that calls the service component 

Runs on a separate EC2 Instance.

When deploying on an EC2 server, go to index.html file and change the src where href = `http://localhost:3001` to Public DNS address of the deployed server

Setup port forwarding to port 3000 
sudo iptables -t nat -A PREROUTING -i eth0 -p tcp --dport 80 -j REDIRECT --to-port 3000

Start node process

