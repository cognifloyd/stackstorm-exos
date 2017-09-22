# EXOS Integration Pack

This pack allows you to run commands against Extreme EXOS-based devices

## Configuration

Copy the example configuration in [exos.yaml.example](./exos.yaml.example)
to `/opt/stackstorm/configs/exos.yaml` and edit as required.

It must contain:

* ``username`` - Email of the account being used for the integration
* ``password`` - An API token generated in the admin interface

You can also use dynamic values from the datastore. See the
[docs](https://docs.stackstorm.com/reference/pack_configs.html) for more info.

**Note** : When modifying the configuration in `/opt/stackstorm/configs/` please
           remember to tell StackStorm to load these new values by running
           `st2ctl reload --register-configs`

## Actions

* ``cmd`` - Run a list of commands against an EXOS device
