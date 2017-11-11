# ansible-options-example
An ansible example showing application options overridden by defaults

## Purpose

To see how we can define common options across multiple applications
in a single structure, and have the ability to provide default options
if they aren't specified by the application.

See [options-with-defaults/vars/main.yml](options-with-defaults/vars/main.yml) 
to get an idea of the structure in use.

There are 3 applications defined.

application_1 provides all options and nothing should be overriden.
application_2 provides only 1 option - the rest should be filled in by the defaults.
application_3 doesn't define any options, so the defaults should be used.

## Running
```
ansible-playbook playbook.yml
```
