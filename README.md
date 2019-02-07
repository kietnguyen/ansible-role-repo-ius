# Ansible Role: IUS Repository

[![Build Status](https://travis-ci.org/kietnguyen/ansible-role-repo-ius.svg?branch=master)](https://travis-ci.org/kietnguyen/ansible-role-repo-ius)

Install [IUS's RPM repository](https://ius.io/) for CentOS.

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    ius_repo_url: "https://centos{{ ansible_distribution_major_version }}.iuscommunity.org/ius-release.rpm"

The URL from which the IUS repo `.rpm` will be downloaded and installed.

    ius_repo_gpg_key_url: "https://dl.iuscommunity.org/pub/ius/IUS-COMMUNITY-GPG-KEY"

IUS repo GPG key location. Can be set to a local file or to the URL from IUS's website.

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - kietnguyen.repo_ius

## License

MIT / BSD

## Author Information

This role was created in 2019 by Kiet Nguyen.
