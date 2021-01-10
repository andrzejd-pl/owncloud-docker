# owncloud docker

This is example configuration of [owncloud](https://owncloud.com/) running on [Docker](https://www.docker.com/) with HTTPS.

## How to use

To use it you must:
1. Generate SSL cert using [certbot](https://certbot.eff.org/), e.g. `sudo certbot certonly --manual --preferred-challenges dns`
2. (If you haven't) Generate dhparams (see in google how to do). 
3. Fill `ADMIN_USERNAME`, `ADMIN_PASSWORD` and `OWNCLOUD_DOMAIN` environment variables in `.env` file.
4. Replace `domain.com` to your domain in `nxinx-conf/default.conf` file.
