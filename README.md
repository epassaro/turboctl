# turboctl
script to control AMD Turbo Core via systemd service

## Installation

1. copy `disable-turbo-core.service` file into `/etc/systemd/system/` folder
2. run `$ sudo systemctl daemon-reload`
3. run `$ sudo systemctl start disable-turbo-core.service`
4. run `$ chmod u+x turboctl`
5. copy `turboctl` script in `$HOME/bin` folder


## Usage

```
usage: turboctl [-h] [-s] [-e] [-d]

a script to control AMD Turbo Core via systemd service

optional arguments:
  -h, --help     show this help message and exit
  -s, --status   show current status
  -e, --enable   enable turbo core
  -d, --disable  disable turbo core
```