# GitHub Codespaces + Laravel

This Codespace has everything you need to start exploring the [Laravel Framework](https://laravel.com/).

## Specs

||||
| - | - | - |
| **Container Definition** | [PHP & MariaDB](https://github.com/microsoft/vscode-dev-containers/tree/main/containers/php-mariadb) (MySQL compatible) | `php 8.2-bullseye` |
| **Extensions** |||
|| [SQLTools](https://vscode-sqltools.mteixeira.dev/en/home/) Database management for VS Code | `mtxr.sqltools` |
| | SQLTools [MySQL Driver](https://vscode-sqltools.mteixeira.dev/en/drivers/my-sql/) | `mtxr.sqltools-driver-mysql` |

## Getting Started

Optionally customize the database environment variables in `docker-compose.yml`. All values are set to `mariadb` by default:

```yml
db:
    # ...

    environment:
      MYSQL_ROOT_PASSWORD:
      MYSQL_DATABASE:
      MYSQL_USER:
      MYSQL_PASSWORD:
```

Then apply those values in your `.env` file:

```env
DB_DATABASE=
DB_USERNAME=
DB_PASSWORD=

Finally, migrate and seed your database:

```sh
php artisan migrate
php artisan db:seed
```

### Building the project

To bundle your assets

```sh
npm run dev
```

To bundle your assets for production

```sh
npm run build
```

To serve your project

```sh
php artisan serve
```
> Github Codespaces will automatically [forward ports](https://docs.github.com/en/codespaces/developing-in-codespaces/forwarding-ports-in-your-codespace) so you can view the running project on your local machine.
