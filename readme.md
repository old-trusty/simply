simply:

ask    prompt user for input with defaults
  -h, --help
  -p, --parse      common regex to compare to
  -d, --nodefault  return "" on prompt: ""enter
  -e, --noescape   just return on escape instead of exiting
  
build  build common textual constructs
  -a, --arg-capsule    `[y/N/m]` style builder that takes options and default and returns capsule and passed options
