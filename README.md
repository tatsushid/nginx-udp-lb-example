NGINX UDP Load Balancing Example
================================

This is just an example for testing NGINX UDP load balancing functionality
newly added since NGINX 1.9.13.

## How to try

1. Clone this repository
2. Run `docker-compose up`
3. Check your docker machine IP address: `docker-machine ip your-machine`
4. Send a query resolving `example.com` to your docker machine IP address
   
   ```
   dig @your-machine-ip-addr example.com +short
   ```
   
   `127.0.0.10` and `127.0.0.20` should be displayed alternately.
