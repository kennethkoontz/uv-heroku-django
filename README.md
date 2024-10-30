# UV with Heroku and Django

This project uses the UV package manager to manage the dependencies of a Django project and demonstrates deployment to heroku using heroku's container stack (Docker).

## Deploying to heroku

### Login to heroku

```bash
heroku login
```

### Create heroku container app

```bash
heroku create --stack=container
```

### Push to heroku

```bash
git push heroku main
```

### Open in heroku

```bash
heroku open
```

If deployment was successful you should see the Django welcome page.

## References

Here are some references used to make this project.

- [Building Docker Images with heroku.yml](https://devcenter.heroku.com/articles/container-registry-and-runtime)
- [UV w/Docker](https://docs.astral.sh/uv/guides/integration/docker/#installing-uv)
- [UV w/Django](https://blog.pecar.me/uv-with-django#installing-dependencies-in-ci)
