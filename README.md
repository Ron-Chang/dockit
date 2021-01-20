# Dockit
## - What is this?
Fuzzy the current location or appoint specific project name to
- git
  + pull repository and all submodules

- docker
  + launch the same prefix service with current project
  + close the same prefix service with current project
  + execute the container with the same as project


## - How to install
```bash
pip install dockit
```

## - How to use

### CLI

```bash
dockit [-h] [-n PROJECT_NAME] [-p] [-s] [-l] [-u] [-e] [-d] [-c]
```

#### -h, --help
> show this help message and exit

#### -n, --project-name
> appoint specific project name

#### -p, --git-pull
> pull git repository and all sub repositories

#### -l, --docker-launch-service
> parse project prefix and launch ${PREFIX}_service

#### -u, --docker-up-container
> docker-compose up -d container

#### -d, --docker-down-container
> docker-compose down container

#### -c, --docker-close-service
> parse project prefix and close ${PREFIX}_service

#### -e, --docker-exec-container
> docker exec -it container bash

#### -s, --docker-show-containers
> show docker processes

If you like my work, please consider buying me a coffee or [PayPal](https://paypal.me/RonDevStudio?locale.x=zh_TW)
Thanks for your support! Cheers! 🎉
<a href="https://www.buymeacoffee.com/ronchang" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" align="right"></a>
