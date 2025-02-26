# Automatic Ripping Machine (ARM) - Development Tools

## Overview

Development tools to help automate testing and fault finding when making changes the ARM main code.
Aim of this code is to be independant of the main ARM Repo, such that no libraries are pulled into support the test code. With the intent that it is possible to run the ARM Devtools as a standalone python script. This is to avoid introducing errors into the main code from the test tool.
Currently a work in progress.

## Features

- Manage branch changes and the ARMUI
- Clear data from the ARM main folder (/home/arm)
- Database management
    - Remove the database file, test running of ARM on a new system
    - Roll the database back a version, usefull for testing database migrations
    - Populate the database with generic data for testing



## Usage

$python3 armdevtools.py -h
usage: armdevtools.py [-h] [-b B] [-d] [-db_rem] [-db_roll DB_ROLL] [-db_data] [-v]

Automatic Ripping Machine Development Tool Scripts

options:
  -h, --help        show this help message and exit
  -b B              Name of the branch to move to, example -b v2_devel
  -d                Clear the arm home folder, remove all directories and files
  -db_rem           Database tool - remove current arm.db file
  -db_roll DB_ROLL  Database tool - roll the current database back a version,input number of versions to roll
                    back.
  -db_data          Database tool - populate the database with Lorem Ipsum data. Requires the active database to
                    be the most current
  -v                ARM Dev Tools Version


## Requirements

- Same as the main ARM repo


## Install

No install required, once ARM installed

## Troubleshooting
 Please see the [wiki](https://github.com/automatic-ripping-machine/automatic-ripping-machine/wiki/).

## Contributing

Pull requests are welcome.  Please see the [Contributing Guide](https://github.com/automatic-ripping-machine/automatic-ripping-machine/wiki/Contributing-Guide)

If you set ARM up in a different environment (hardware/OS/virtual/etc.), please consider submitting a howto to the [wiki](https://github.com/automatic-ripping-machine/automatic-ripping-machine/wiki).

## License

[MIT License](LICENSE)
