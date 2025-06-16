# simply

simple command line scripting toolbox

```help
usage: simply [options] <tool> ...

options:
    -h, --help
        print this message.  

tools:
    -a, ask
        prompt user for input and return it with escape exiting.
    -b, build
        build common textual constructs. many of which made for use with ask.
```
##  simply ask

prompt user for input with default on empty enter and exit on escape.
simply ask    prompt user for input with defaults

```help
usage: simply ask [options] <prompt> <default> <other>...

options:
    -h, --help
        print this message.
    -p, --parse
common regex to compare to
    -n, --nodefault
        dont return default on empty enter
    -d, --dmenu
        show <other> options to complete and highlight the <default> in the style of dmenu / fzf.
    -e, --noexit
        dont die when escape pressed 
    -y, --add-to-options
        use fallback <default> and <others> with supplied extra <others>.

arguments:
    <prompt>
        what to ask the user before there input.
    <default>
        the answer to return when the user submits no input.
    <other>
        the rest of the answers that can be prompted dmenu style.
```

## simply build 

build common textual constructs

```help
usage: simply build [options] <construct> ...

options:
    -h, --help
        print this message.  

construct:
    capsule <default> <all>
        build  [Y/n/m] from "simply build capsule yes yes no maybe" for use with "simply ask" that takes options and default and returns capsule and passed options.
    regex
        build a regex match that matches the first letter to the last letter with any capitalization.
```
