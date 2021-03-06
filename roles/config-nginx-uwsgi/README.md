Role Name
=========

A brief description of the role goes here.

Requirements
------------


Role Variables
--------------

- `APP_BASE_DIR` - the base, or root, directory of the application
- `UWSGI_APP_NAME` - the name of the enabled UWSGI application
- `UWSGI_APPS_ENABLED_PATH` - path to enabled apps, default `/etc/uwsgi/apps-enabled/`
- `UWSGI_INI_SRC_NAME` (optional) - file name, including relative path from `APP_BASE_DIR`

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```
    - hosts: all
      roles:
        - { role: config-nginx-uwsgi,
            APP_BASE_DIR: "{{ TROPOSPHERE_LOCATION }}",
            UWSGI_APP_NAME: 'troposphere',
            tags: ['troposphere'] }
```

or

```
    - hosts: all
      roles:
        - { role: config-nginx-uwsgi,
            APP_BASE_DIR: "{{ ATMOSPHERE_LOCATION }}",
            UWSGI_APP_NAME: 'atmosphere',
            tags: ['atmosphere'] }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
