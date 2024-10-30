# UV with Heroku and Django

This project demonstrates deploying a django app using the UV package manager to Heroku.

[!IMPORTANT]
Why? Heroku's python buildpack doesn't support UV at this moment so in order to use UV with Heroku, Heroku's container stack (docker) is required.

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
