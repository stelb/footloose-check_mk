# CheckMK Installation with footloose

## Requirements

* docker
* [footloose](https://github.com/weaveworks/footloose)
* ansible

## setup

    git clone --recursive https://github.com/stelb/footloose-checkmk.git
    cd footloose-checkmk
    footloose create
    ansible-playbook site.yml

now checkMK is running with webserver port forwarded to some random port on localhost

    footloose status

site test is created with user cmkadmin password test

Access via:

    http://localhost:<aboveport>/test/
