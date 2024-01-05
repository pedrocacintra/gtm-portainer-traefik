# gtm-portainer-traefik
Install GTM server container on a VPS with Portainer + Traefik

# # Installation steps:
1) Create 2 (A) DNS records pointing your VPS IP, one for the main tag server, and the other for the preview server. (Ex: gtm.domain.com and gtm-preview.domain.com)
2) Create network for the GTM stack
3) Connect the created network to Traefik's container
4) Create stack, paste the .yaml code, upload the .env and change to your info (urls, container and network name)
5) Deploy the stack

# # Testing:
1) Try opening both of the urls with a /healthz in the end, (ex: https://gtmpreview.domain.com/healthz and https://gtm.domain.com/healthz). You should see a black page with the text "ok".
2) Go to the GTM container and click on preview, this should open the preview screen correctly.
