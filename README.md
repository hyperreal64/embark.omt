# Embark for Oh My Tmux

![embark-omt-demo.png]

## How to use

Required: [Oh my tmux!](https://github.com/gpakosz/.tmux)

Ensure the config directory exists for Oh my tmux and its themes:

```bash
mkdir -p ~/.config/oh-my-tmux/themes
```

Now clone this repository and copy `embark.conf`:

```bash
git clone https://github.com/hyperreal64/embark.omt.git
cd embark-omt-theme/
cp -v embark.conf ~/.config/oh-my-tmux/themes/
```

In `~/.tmux.conf.local`, set the theme to embark:

> Note that this overrides some options in vanilla `~/.tmux.conf.local`, so place these lines after the `display` section.

```bash
# theme loader
themes_folder='$OH_MY_TMUX/themes/'

# embark theme
theme="embark.conf"

if "[ -d ${themes_folder} ]" "source ${themes_folder}${theme}"
```

## License

[MIT License](https://github.com/hyperreal64/embark-omt-theme/blob/master/LICENSE)
