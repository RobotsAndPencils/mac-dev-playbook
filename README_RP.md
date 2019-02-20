1. Clone `mac-dev-playbook` (allow macOS to install git via command line tools, but don't install xcode)
2. Configure ssh per GitHub and add ssh key to robotbuildbox GitHub account
3. Install ansible globally on this Mac per https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#latest-releases-on-macos

```
$ sudo easy_install pip
$ sudo pip install ansible
```

4. Run `$ ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
5. Run `$ ansible-playbook main.yml -i inventory -K` inside this directory. Enter your account password when prompted. This will leverage our customized config (which likely still needs customization)

