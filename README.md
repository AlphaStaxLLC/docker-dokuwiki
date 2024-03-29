# docker-dokuwiki

Docker container for [Dokuwiki][3]

"DokuWiki is a simple to use and highly versatile Open Source [wiki][6] software that doesn't require a database. It is loved by users for its clean and readable [syntax][7]. The ease of maintenance, backup and integration makes it an administrator's favorite. Built in [access controls][8] and [authentication connectors][9] make DokuWiki especially useful in the enterprise context and the large number of [plugins][10] contributed by its vibrant community allow for a broad range of use cases beyond a traditional wiki."

## Install dependencies

  - [Docker][2]

To install docker in Ubuntu 14.04 use the commands:

    $ sudo apt-get update
    $ sudo apt-get install docker.io

 To install docker in other operating systems check [docker online documentation][4]

## Usage

To run container use the command below:

    $ docker run -d -p xxxx:80 quantumobject/docker-dokuwiki

Check port and point your browser to http://[ip]:xxxx/install.php  to initially configure your DokuWiki.

when done please execute this command for security and remove the install script:

    $ docker exec -it container_id after_install

## More Info

About dokuwiki[www.dokuwiki.org][1]

To help improve this container [quantumobject/docker-dokuwiki][5]

[1]:https://www.dokuwiki.org
[2]:https://www.docker.com
[3]:http://download.dokuwiki.org/
[4]:http://docs.docker.com
[5]:https://github.com/QuantumObject/docker-dokuwiki
[6]:http://en.wikipedia.org/wiki/Wiki
[7]:https://www.dokuwiki.org/wiki:syntax
[8]:https://www.dokuwiki.org/acl
[9]:https://www.dokuwiki.org/auth
[10]:https://www.dokuwiki.org/plugins
