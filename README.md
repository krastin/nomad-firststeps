# nomad-firststeps
A repository to test and learn about Nomad

# How to Use

## Basic setup

    vagrant up
    vagrant ssh
    sudo nomad agent -dev
    nomad job start /vagrant/example.nomad

## Cluster-like setup

    vagrant up
    vagrant ssh
    nomad agent -config /vagrant/server.hcl
    nomad agent -config /vagrant/client1.hcl
    nomad agent -config /vagrant/client2.hcl
    nomad job start /vagrant/example3.nomad

