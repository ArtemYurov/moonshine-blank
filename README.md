# MoonShine 3 blank project

---

| Settings                         |
|----------------------------------|
| ✅ Enable authentication          |
| ✅ Install with system migrations |
| ⛔ Enable notifications           |
| ✅ Base theme                     |

---

| Included        |
|-----------------|
| ✅ Basic setting |
| ✅ PhpStan       |
| ✅ Php CS Fixer  |
| ✅ Rector        |
| ✅ TypeScript    |
| ✅ Xdebug        |
| ✅ Docker        |

## Installation
- Run the git clone command `git clone git@github.com:dev-lnk/moonshine-blank.git .`.
- Copy the `.env.example` file and rename it to `.env`, customize the `#Docker` section to your needs.
- Run the command `make build`, and then `make install`.
- Check the application's operation using the link `http://localhost/admin` or `http://localhost/admin:${APP_WEB_PORT}`.
- Run stat analysis and tests using the command `make check`.

## About
This is a Blank Moonshine 3 based on the [laravel-blank](https://github.com/dev-lnk/laravel-blank) project.

## Docker

### Images

- nginx:1.29-alpine
- php:8.4-fpm (with xdebug)
- mysql:9.4 or postgres:16.2
- redis:8.2.0-alpine
- node:24.5-alpine3.22

### Other
- Many commands to speed up development and work with docker can be found in the `Makefile`
- If you don't need Docker, remove: `/docker`, `docker-compose.yml`, `Makefile`. Convert `.env` to standard Laravel form
- To launch containers with `worker` and `scheduler`, delete comments on the corresponding blocks in `docker-compose.yml`
