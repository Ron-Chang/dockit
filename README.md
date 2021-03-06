# Dockit
## - What is this?

docker
> To launch, close and execute container with docker-compose and its relative services without change the directory.

git
> Fuzzy the current location to pull all the submodules and specify the project if required.

## - History

|#|      date|                                            version|
|-|----------|---------------------------------------------------|
|1|2020/01/24| [v0.1.2](https://github.com/Ron-Chang/dockit#v012)|
|2|2020/01/27| [v0.1.4](https://github.com/Ron-Chang/dockit#v014)|
|3|2020/02/02| [v0.1.5](https://github.com/Ron-Chang/dockit#v015)|
|4|2020/02/13| [v0.1.6](https://github.com/Ron-Chang/dockit#v016)|
|5|2020/03/22| [v0.1.8](https://github.com/Ron-Chang/dockit#v018)|

#### v0.1.2
- Fixed dockit -u & -d cannot work properly when the project not located at $HOME directory.
#### v0.1.4
- Replaced whole color module.
#### v0.1.5
- Fixed display bug while remote added new branches.
- Removed optional argument `-n`, use positional argument instead.(default:basename of $pwd)
#### v0.1.6
- Support pull a project and the all the submodules which belongs to the project without change the directory.
- Support change source directory by setting a environment variable `export DOCKIT_ROOT='~/your/custom/path'`.
#### v0.1.8
- Removed -l flag of _exec_container to solve some container cannot call go properly

## - How to install
- Install
```bash
pip install dockit
```
- Setup source root(Optional)
Make it temporary or add the following line to your `.bashrc`, `.zshrc` or profile to keep it permanently.
```bash
export DOCKIT_ROOT='~/TO/YOUR/CUSTOM/PATH'
```

## - How to use

```bash
dockit.py [-h] [-a] [-p] [-l] [-c] [-u] [-d] [-e] [-s] [project]
```

#### -h, --help
> show this help message and exit

#### -p, --git-pull
> pull git repository and all sub repositories

#### -l, --docker-launch-service
> parse project prefix and launch ${PREFIX}_service

#### -u, --docker-up-service
> docker-compose up -d container with the same name as project

#### -a, --docker-attach-container
> to keep attaching mode after docker-compose upped

#### -d, --docker-down-service
> docker-compose down container with the same name as project

#### -c, --docker-close-service
> parse project prefix and close ${PREFIX}_service

#### -e, --docker-exec-container
> docker exec -it container bash

#### -s, --docker-show-containers
> show docker processes

```bash
# .bashrc or .zshrc
alias gitpull="dockit -p"
alias run="dockit -e"
alias up="dockit -u"
alias uu="dockit -l"
alias uuu="dockit -lu"
alias uur="dockit -lue"
alias uura="dockit -luea"
alias down="dockit -d"
alias dd="dockit -c"
alias ddd="dockit -cd"
alias dps="dockit -s"
```

If you like my work, please consider buying me a coffee or [PayPal](https://paypal.me/RonDevStudio?locale.x=zh_TW)
Thanks for your support! Cheers! 🎉
<a href="https://www.buymeacoffee.com/ronchang" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" align="right"></a>
