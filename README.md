# Docker Spotweb

## Retrieve spots

`sudo docker compose exec -it -u root app sh`:

```bash
$ crontab -e
*/15 * * * * su -l tea -s /usr/local/bin/php /src/app/retrieve.php
10 */1 * * * su -l tea -s /usr/local/bin/php /src/app/bin/check-cache.php
```
