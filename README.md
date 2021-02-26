The media stack is composed of:

- jackett (ntz listing)
- flaresolverr (bypass cloudflare)
- sonarr (torrent & metadata DB search)
- transmission (torrent download)
- jellyfin (media hosting)

Use `docker-compose up -d` to start.

The repository contains only necessary files, as of `.gitignore`, other files might be created at first run, they should NOT be committed.

More specifically, only service configs are committed, except of user list of jellyfin and password of transmission.

`downloads/` MUST be mounted to store media files, ideally on a large disk.
