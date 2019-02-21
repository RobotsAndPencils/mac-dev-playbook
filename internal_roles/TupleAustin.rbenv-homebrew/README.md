# Ansible Role: rbenv with Homebrew

Installs rbenv, ruby-build, Ruby, and Bundler (globally) via Homebrew on macOS.

For simplicity, the installed Ruby version and gems are specific to the current user.

## Role Variables

The default Ansible variables and values are:

```yaml
# See: defaults/main.yml
rbenv_homebrew:
  ruby_version: 2.3.1
```

`ruby_version` indicates which version of Ruby is to be installed with `rbenv install`.

## Example Playbook

```yaml
- hosts: localhost
  vars:
    rbenv_homebrew:
      ruby_version: 2.3.1
  roles:
    - TupleAustin.rbenv-homebrew
```

## License

MIT.
