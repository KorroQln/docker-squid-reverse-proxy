# docker-squid-reverse-proxy

## Tweaking the config
- Disable caching and avoid autogenerating the defaul log folder:
```cache_log /dev/null```
```cache deny all```
- Disable access log(optional):
```access_log none```

## Health Check
- https://stackoverflow.com/questions/60038914/simple-healthcheck-endpoint-in-nginx-server-container
- https://chat.openai.com/share/cc804d14-26c1-4491-b476-1a9f34ea86c5

## Nexus Registry
- https://www.youtube.com/watch?v=tO8nWh38yTU
- https://www.youtube.com/watch?v=dpWxWr90MGI
- https://www.youtube.com/results?search_query=docker+proxy
- https://iamsaleempasha.medium.com/nexus-as-docker-trusted-registry-to-pull-push-docker-images-6f74f599fd9
- https://support.sonatype.com/hc/en-us/articles/115013153887-Docker-Repository-Configuration-and-Client-Connection
Try to execute below Command to login into Docker Nexus Registry
```$ docker login –u <nexususerid> –password ****** <nxs-ipaddr>:<port>```

## References
- https://www.digitalocean.com/community/tutorials/how-to-set-up-squid-proxy-on-ubuntu-20-04
- https://www.devopsschool.com/blog/how-to-configure-http-proxy-with-docker/
- https://hub.docker.com/r/ubuntu/squid
- https://hub.docker.com/r/scbunn/squid
- https://fariszr.com/en/squid-proxy-docker-setup/
- https://willsena.dev/building-a-squid-proxy-container-to-test-npm-with-http-proxy/
- https://cloudinfrastructureservices.co.uk/how-to-setup-squid-proxy-docker-container-image/
- https://stefan-poeltl.medium.com/setup-a-web-proxy-server-with-docker-d5c6942b5575
- https://webhostinggeeks.com/howto/how-to-install-squid-proxy-server-in-docker-containers/#:~:text=Using%20a%20Squid%20Proxy%20Server,a%20secure%20and%20efficient%20manner.
- https://stefan-poeltl.medium.com/setup-a-web-proxy-server-with-docker-d5c6942b5575
- https://movidius.github.io/ncsdk/docker_proxy.html
