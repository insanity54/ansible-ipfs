# ansible-ipfs

[![Build Status](https://travis-ci.org/insanity54/ansible-ipfs.svg?branch=master)](https://travis-ci.org/insanity54/ansible-ipfs)

Quick and easy playbook for installing an IPFS node/gateway as a service

If you are looking for a way of using Ansible to deploy and manage a cluster of ipfs nodes/gateways meant for pinning and serving content, you might like my other project, [ipfs-kloud](https://github.com/insanity54/ipfs-kloud)


## What it does

* extract and copy pre-built ipfs binary to /usr/local/bin/ipfs
* create ipfs system service (files/ipfs.conf)
* run ipfs service
  * ipfs daemon runs using standard ports 4001, 5001, 8080



## What it does not do

* set up FUSE


## Future potential

* use gx to download and install ipfs
* use gx webhooks to make a GitHub README.md badge showing whether or not this repo is using the latest stable ipfs


## Credits

The ipfs init script used in this project was originally written by [dylanPowers](https://github.com/dylanPowers) from the [ipfs-linux-service](https://github.com/dylanPowers/ipfs-linux-service) project. ansible-ipfs made one change-- where the ipfs daemon saves it's logs to. (/var/log/ipfs.log instead of /var/lib/ipfs/daemon.log)


## Contributing

Pull requests and new issues are very much appreciated!
