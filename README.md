# masc

A malware (web) scanner developed during [CyperCamp](http://www.cybercamp.es) Hackathon 2017

## About

[homepage](https://sfaci.github.io/masc)

## Features

* Scan any website for malware using OWASP WebMalwareScanner checksum and YARA rules databases
* WordPress support
..* Scan your site to know if it has been infected with some malware
..* Clean up your site to avoid giving extra information to attackers
..* Backup your site (to recover later if you need)
--* List your local backups
..* Logging support

## Usage

```bash
usage: masc.py [-h] [--site-type {wordpress,drupal,joomla,magento}]
               [--scan PATH] [--name NAME] [--list-backups]
               [--add-file FILENAME] [--add-word STRING] [--clean-up]

optional arguments:
  -h, --help            show this help message and exit
  --site-type {wordpress,drupal,joomla,magento}
                        which type of web you want to scan:: wordpress,
                        joomla, drupal or magento
  --scan PATH           Scan an installation at the given PATH
  --name NAME           Name assigned to the scanned installation
  --list-backups        List local backups
  --add-file FILENAME   Add a suspect file to the dictionary
  --add-word STRING     Add a suspect content to the dictionary
  --clean-up            Clean up the site to hide information to attackers
```

## Documentation

[wiki](https://github.com/sfaci/masc/wiki)

## Thanks

Thanks to [OWASP WebMalwareScanner](https://github.com/maxlabelle/WebMalwareScanner) for some ideas and the signatures databases with checksums and YARA
rules (and how to load it to work with). 

## Author

Santiago Faci <santiago.faci@gmail.com>
