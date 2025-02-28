Provide your solution here:
* Install process-exporter to gather metrics and identify root cause of memory leak. It may come from nginx or from the other application.
* If the memory leak is from the other application, we can use move this application out of server.
* If high memory consumption from nginx, we have to use nginx-exporter to gather metrics and identify the root cause. There are 2 scenarios:
  * If the memory leak is from nginx, we can try to upgrade nginx to the latest stable version.
  * If the memory consumption because of high traffic, we can try to use CDN to reduce the traffic to the server. Also create multiple instances of nginx and use load balancer to distribute the traffic.