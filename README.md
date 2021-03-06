[![](https://images.microbadger.com/badges/version/kukielka/cloudflare-ddns.svg)](https://microbadger.com/images/kukielka/cloudflare-ddns "Get your own version badge on microbadger.com") [![](https://images.microbadger.com/badges/image/kukielka/cloudflare-ddns.svg)](https://microbadger.com/images/kukielka/cloudflare-ddns "Get your own image badge on microbadger.com")

[![](https://www.cloudflare.com/img/logo-cloudflare-dark.svg)](https://www.cloudflare.com/ "The collective knowledge of 5,500,000 websites powers a new kind of security")



# cloudflare-ddns
This Dockerfile will keep your Docker containers public IP address up to date with a CloudFlare DNS A record (Dynamic DNS).

*(Based on the work of Marcus Hughes <hello@msh100.uk to better fit UNRAID)*


**Usage:**



To use, run the Docker container with your CloudFlare API credentials found on your CloudFlare account page:

docker run --net="host" --name="cloudflare" -e "CF_EMAIL=your@cloudflare_email.com" -e "CF_HOST=sub.domain.com" -e "CF_API=xxxxxxxxxxxxxx" -e "CF_PROXY=true/false" kukielka/cloudflare-ddns

To run in the background, add the -d switch after docker run.
