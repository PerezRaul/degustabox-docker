# Requirements

- [Docker](https://www.docker.com/products/docker-desktop)

# Installation

Clone this repository on _~/Sites_ with _docker_ name and follow this instructions:

---

1 - Add aliases to your _.bash_profile_ or _.zshrc_:

```shell
alias dockerup="~/Sites/docker ; docker-compose up mysql nginx php-fpm rabbitmq docker-in-docker redis workspace"
alias dockerdown="~/Sites/docker ; docker-compose down"
alias dockerbash="~/Sites/docker ; docker-compose bash"
alias dockerbuild="~/Sites/docker ; docker-compose build mysql nginx php-fpm rabbitmq docker-in-docker redis workspace"
```

---

2 - Restart your terminal or execute:

```shell
#.zshrc
> source ~/.zshrc

#.bash_profile
> source ~/.bash_profile
```

---

3 - Copy the .env.example file:
```shell
> cp .env.example .env
```

---

3 - Build containers and start with the following commands:

```shell
> dockerup
```

---

# Working

All you need in order to install composer dependencies or what else the project need is enter on the workspace container with that command:

---

```shell
> dockerbash
```

---

# Shortcuts

- [RabbitMQ](http://localhost:15672) (guest:guest)
