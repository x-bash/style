# style

To collect all kinds of style in bash

```bash
# Using el style
eval "$(curl https://x-bash.github.io/style/el)"

# Using tomorrow night style
eval "$(curl https://x-bash.github.io/style/tomorrow-night)"

eval "$(curl https://x-bash.github.io/style/apple-pro)"
```

# Initialize when bash ready

Edit $HOME/.bashrc, add the code beside

```bash

```

If you are already initialize x-bash, just using

```bash
@src style/el
```

**What if I want style without x-bash**

Add the following one-line-code in your bash_rc

```bash
STYLE="DEFAULT_STYLE" D="$HOME/.x-cmd.com/x-bash/style/$DEFAULT_STYLE" eval '[ -e $D ] || mkdir -p $(dirname $D) && curl "https://x-bash.github.io/style/$DEFAULT_STYLE" >$D && source $D'
```

Replace the DEFAULT_STYLE to your prefered style


# TODO

1. Write a style manager, easily to switch between style
2. Enrich this document

