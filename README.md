# aws-vpn-client-docker
 with AWS VPN SAML.

## How to use

### Use a prebuilt container
1. CloseDownload your AWS VPN client profile into a directory and rename it as "vpn.conf"
2. Build the dockerfile: docker build . -t vpn:latest
3. MV the "launchVPN" into your path (ex: /bin/launchVPN)
4. Everytime you want to execute. Type in the command line: "launchVPN"


> [!IMPORTANT]
> This repository is largely simply packaging other authors' work!
> 
> ## Credits
> ### [rdvencioneck/aws-vpn-client-docker](https://github.com/rdvencioneck/aws-vpn-client-docker)
> He created a dockerfile for Alex's solution. I just added a couple of extra features on top of that.
> ### [samm-git/aws-vpn-client](https://github.com/samm-git/aws-vpn-client)
> 
> Alex Samorukov is the mastermind behind this implementation. He figured out how AWS patches the openvpn client and
> created the first implementations. Be sure to read his [blog](https://smallhacks.wordpress.com/2020/07/08/aws-client-vpn-internals/)
> on for more details.
> 
> ### [botify-labs/aws-vpn-client](https://github.com/botify-labs/aws-vpn-client)
> 
> Botify Labs maintains the `.patch` files for more recent versions of OpenVPN than what are available originally
> in Alex's repository.

---
