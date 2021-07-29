My notes on

[github - aschmelyun/docker-compose-laravel](https://github.com/aschmelyun/docker-compose-laravel.git)

based on the YouTube videos:

[Create a local Laravel dev environment with Docker](https://youtu.be/5N6gTVCG_rw)

[A much better local Laravel dev environment with Docker](https://youtu.be/I980aPL-NRM)

1. Run `docker-compose up -d --build` - this will create a few directories
2. In the newly created `/src/.env` change the following settings:

- DB_HOST=mysql
- DB_DATABASE=homestead
- DB_USERNAME=homestead
- DB_PASSWORD=secret

3. Run `docker-compose run --rm artisan migrate`
4. Run `docker-compose run --rm npm install`

---

When done run

`docker-compose down`

---

To return to work run

`docker-compose run -d`

---

If you need to run **_composer_**, **_artisan_**, or **_npm_** for anything in this project, just put

`docker-compose run -rm`

before the command and you're set.
