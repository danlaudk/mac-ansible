mac-ansible
===========

I use this project to configure my macOS the way I like it. 
Includes role to install jenv and openjdk
Forked from [blog post](https://adamj.eu/tech/2019/03/20/how-i-provision-my-macbook-with-ansible/).

Getting Started
---------------

1. Install [homebrew](http://brew.sh/) with the command from the site
2. `brew install pyenv`
3. `pyenv install <latest_python_version>` (Check playbook up to date)
4. Make sure pyenv's python on path (it will be after my shell settings are in place from playbook)
5. `python -m venv venv`
6. `source venv/bin/activate`
7. `pip install ansible` (always the best way to install Ansible)
8. `ansible-galaxy install -r roles/requirements.yml`
6. Then `ansible-playbook -K ./playbook.yml`   (-K prompts for sudo password)

Fork! Copy! Adapt!
------------------

This is distributed under the Unlicense so you can do whatever you want with
it, see LICENSE.
