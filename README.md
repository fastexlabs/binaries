# Caravan Binaries and Management Script

This repository provides a management script for the Bahamut blockchain execution layer - Caravan. The management script simplifies the process of downloading, installing, and managing the Bahamut execution layer, making it easy to set up and maintain a Caravan node. Precompiled binaries for Caravan are available as tagged releases in the binaries repository.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Commands](#commands)
- [Options](#options)
- [Support](#support)
- [License](#license)

## Prerequisites

Ensure that you have the following prerequisites installed on your system:

- [Curl](https://curl.se/download.html) and [Wget](https://www.gnu.org/software/wget/)
- [pidof](https://formulae.brew.sh/formula/pidof)

## Installation

1. Download the `bahamut` management script:

```bash
git clone
chmod +x bahamut
```

2. Run the management script to download and install the Caravan execution layer:

```bash
./bahamut install
```

This command will download the latest Caravan binaries from the tagged releases in the execution layer repository. After the install added Bahamut/sahara/sahara_config.toml and Bahamut/oasis/oasis_config.toml config files, in which you can change ports.

## Usage

Once you have installed the Caravan execution layer, you can use the bahamut script to manage your Caravan node. The following commands are available:

`./bahamut start`: Starts the Caravan node.\
`./bahamut stop`: Stops the Caravan node.\
`./bahamut restart`: Restarts the Caravan node.\
`./bahamut status`: Returns the status of the Caravan node.\
`./bahamut install`: Installs Caravan dependencies needed for the start.\
`./bahamut update`: Updates Caravan binaries and native scripts.\

## Commands

### Start the Caravan Node
To start the Caravan node, run:

```bash
./bahamut start --network sahara
```

### Stop the Caravan Node
To stop the Caravan node, run:

```bash
./bahamut stop
```

### Restart the Caravan Node
To restart the Caravan node, run:

```bash
./bahamut restart
```

### Check the Caravan Node Status
To check the status of the Caravan node, run:
```bash
./bahamut status
```

### Install the Caravan Node Dependencies
To install Caravan dependencies needed for the start, run:
```bash
./bahamut install
```

### Update the Caravan Node
To update the Caravan node, run:
```bash
./bahamut update
```

## Options

- `--help`: Show help information and a list of available commands.
- `--network`: Specify the network to connect the Caravan node to, e.g., `--network sahara` or `--network oasis`.

## Support

If you encounter any issues or have any questions, please open an issue on the [GitHub repository](https://github.com/fastexlabs/binaries/issues).

## License

Caravan is released under the [MIT License](https://opensource.org/licenses/MIT). See the [LICENSE](LICENSE) file for more information.
