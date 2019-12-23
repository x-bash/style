# style

To collect all kinds of style in bash

```bash
# Using el style
eval "$(curl https://x-bash.github.io/style/el)"

# Using tomorrow night style
eval "$(curl https://x-bash.github.io/style/tomorrow-night)"

eval "$(curl https://x-bash.github.io/style/apple-pro)"
```

## One line installer

```bash
curl https://x-bash.github.io/style/install
# First install x
# Then add in ~/.bashrc: `eval "$(x bash/boot)"`
# Then add in ~/.bashrc: `@src style/el`
```

## Initialize when bash ready

**If you are already initialize x-bash, just using**

To use x-bash

```bash
D="$HOME/.x-cmd.com/x-bash/boot" eval '[ -e $D ] || (mkdir -p $(dirname $D) && curl "https://x-bash.github.io/boot" >$D) && source $D'
```

```bash
eval "$(x bash/boot)" && @run install
```

Then using `@src` to include style/el

```bash
@src style/el
```

**What if I want style without x-bash**

Add the following one-line-code in your bash_rc

```bash
STYLE="DEFAULT_STYLE" D="$HOME/.x-cmd.com/x-bash/style/$DEFAULT_STYLE" eval '[ -e $D ] || (mkdir -p $(dirname $D) && curl "https://x-bash.github.io/style/$DEFAULT_STYLE" >$D) && source $D'
```

Replace the DEFAULT_STYLE to your prefered style

## TODO

1. Write a style manager, easily to switch between style
2. Enrich this document
