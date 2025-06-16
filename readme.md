# simply
simple command line scripting toolbox in the style of charm's [gum](https://github.com/charmbracelet/gum), but with far less dynamism and sparkle

```
simply ask    prompt user for input with defaults
  -h, --help
  -p, --parse                common regex to compare to
  -d, --nodefault            return "" on prompt: ""enter
  -e, --noescape             just return on escape instead of exiting
  -y, --add-to-options       use yes as default and just add supplied options to yes and no
  
simply build  build common textual constructs
  -c, --arg-capsule    `[y/N/m]: ` style builder that takes options and default and returns capsule and passed options
```
