# xewe-os ecosystem

Every firmware is built from reusable pieces, and xewe-os is the modular framework that puts them
together. It is made for development with AI coding assistants. Two commands, `./setup.sh` and
`./run.sh`, take you from an idea to flashed firmware.

<img alt="xewe-os ecosystem: modules, core and custom modules flow into xewe-os from the top, tools enter from the side; xewe-led-os and xewe-chill-os are built on it; the ecosystem is cyan, custom modules gray, products purple" src="ecosystem-4.svg" width="960">

## Repositories

### Ecosystem

* [`xewe-os`](https://github.com/xewe-labs/xewe-os): lightweight OS for ESP32 and Arduino; the template
* [`xewe-os-core`](https://github.com/xewe-labs/xewe-os-core): the XeWeCore library: serial, CLI engine, storage
* [`xewe-os-modules`](https://github.com/xewe-labs/xewe-os-modules): every xewe-os module, fetched by `./setup.sh`
* [`xewe-os-tools`](https://github.com/xewe-labs/xewe-os-tools): the `xewe` CLI: setup, build, flash, test, release

### xewe-led-os

* [`xewe-led-os`](https://github.com/xewe-labs/xewe-led-os): LED strip firmware for ESP32-C3, -C6 and -S3
* [`xewe-led-os-homeassistant`](https://github.com/xewe-labs/xewe-led-os-homeassistant): Home Assistant integration for XeWe LED OS devices

### xewe-chill-os

* [`xewe-chill-os`](https://github.com/xewe-labs/xewe-chill-os): laptop cooling pad firmware (fan, temperature, LED)

Why it is shaped this way: [xewe-os/doc/XEWE_OS_ECOSYSTEM.md](https://github.com/xewe-labs/xewe-os/blob/main/doc/XEWE_OS_ECOSYSTEM.md).
Arduino IDE only? Install `XeWeCore` from the Library Manager and start with the
[`01_Hello`](https://github.com/xewe-labs/xewe-os-core/tree/main/examples/01_Hello) example.
To contribute, read [CONTRIBUTING.md](https://github.com/xewe-labs/.github/blob/main/CONTRIBUTING.md);
a new module starts with a [module proposal](https://github.com/xewe-labs/xewe-os-modules/issues/new?template=MODULE_PROPOSAL.md).
Everything here is GPL-3.0-only unless a repository says otherwise.
