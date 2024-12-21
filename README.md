# PACLI - PHP Asana Command Line Interface

## Latest Version

### Download Latest Version (1.2.6):
https://raw.githubusercontent.com/chrisputnam9/pacli/master/dist/pacli

### Latest Version Hash (md5):
d6c4204996ab2d761f9af22f6e8e451f

## Install PACLI
1. Make sure you have PHP, or [install it if not](http://php.net/manual/en/install.php)

2. Run this code in a download folder or temporary location:

        curl https://raw.githubusercontent.com/chrisputnam9/pacli/master/dist/pacli > pacli
        chmod +x pacli
        sudo ./pacli install

3. Test success by running in a new terminal session:

        pacli version

# Updating
The script will periodically check for updates autmoatically and inform you when an update is
available.

If an update is available, you can run the following to install the update:

    sudo pacli update

# USAGE:

    pacli <method> (argument1) (argument2) ... [options]

    ----------------------------------------------------------------------------------------------------------------------
    | METHOD                 | INFO                                                                                      |
    ----------------------------------------------------------------------------------------------------------------------
    | backup                 | Backup a file or files to the configured backup folder                                    |
    | clear                  | Clear the screen                                                                          |
    | eval_file              | Evaluate a php script file, which will have access to all internal methods via '$this'    |
    | exit                   | Exit the command prompt                                                                   |
    | get                    | GET data from the Asana API.  Refer to https://developers.asana.com/docs/asana            |
    | help                   | Shows help/usage information.                                                             |
    | install                | Install a packaged PHP console tool                                                       |
    | post                   | POST data to the Asana API.  Refer to https://developers.asana.com/docs/asana             |
    | prompt                 | Show interactive prompt                                                                   |
    | update                 | Update an installed PHP console tool                                                      |
    | version                | Output version information                                                                |
    ----------------------------------------------------------------------------------------------------------------------
    To get more help for a specific method:  pacli help <method>

    ----------------------------------------------------------------------------------------------------------------------
    | OPTION                 | TYPE                              | INFO                                                  |
    ----------------------------------------------------------------------------------------------------------------------
    | --allow-root           | (boolean)                         | OK to run as root without warning                     |
    | --api-cache            | (boolean)                         | Whether to cache results                              |
    | --ssl-check            | (boolean)                         | Whether to check SSL certificates with curl           |
    | --stamp-lines          | (boolean)                         | Stamp / prefix output lines with the date and time    |
    | --verbose              | (boolean)                         | Enable verbose output                                 |
    ----------------------------------------------------------------------------------------------------------------------
    Use no- to set boolean option to false - eg. --no-stamp-lines
