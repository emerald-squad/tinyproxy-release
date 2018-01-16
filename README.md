# tinyproxy-release

BOSH release for tinyproxy

It allows setting multiple instances, listening on different ports with different whitelists.

Example: 
 tinyproxy.instances:
  - name: mything
    port: 8888
    allowed_cidr: 0.0.0.0/0
    whitelisted_domains:
    - google.com
    - amazon.com
  - name: myotherthing
    port: 8889
    allowed_cidr: 0.0.0.0/0
    whitelisted_domains:
    - auth0.com