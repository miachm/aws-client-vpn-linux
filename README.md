# aws-vpn-client-docker
 with AWS VPN SAML.

## How to use

1. Clone the repo.
2. Put your AWS VPN client profile into the directory as "vpn.conf"
3. Build the dockerfile: ```docker build . -t vpn:latest ``` 
4. Move the "launchVPN" script into your path (for example: /bin/launchVPN)
5. Everytime you want to execute. Type in the command line: ```launchVPN```
 
## Credits
This repository is largely simply packaging other authors' work!

### [rdvencioneck/aws-vpn-client-docker](https://github.com/rdvencioneck/aws-vpn-client-docker)
 He created a dockerfile for Alex's solution.
### [samm-git/aws-vpn-client](https://github.com/samm-git/aws-vpn-client)
 
 Alex Samorukov is the mastermind behind this implementation. He figured out how AWS patches the openvpn client and
 created the first implementations. Be sure to read his [blog](https://smallhacks.wordpress.com/2020/07/08/aws-client-vpn-internals/)
 on for more details.
 
 ### [botify-labs/aws-vpn-client](https://github.com/botify-labs/aws-vpn-client)
 
 Botify Labs maintains the `.patch` files for more recent versions of OpenVPN than what are available originally
 in Alex's repository.

---
