Ansible playground
==================

This is a place for collected ansible stuff I wrote during expremimenting with playbooks. Might be interesting - at least for me to remember ;)


List of plays
-------------

**link_or_override**: 
Link files from source to dest or use local overrides.

This makes use of filters for unions/differences of lists, set_fact for variable registration and opened my eyes on use of complex datatypes: Ansible parses all variables with jinja2 (For example python methods like split() will work - even on filter expressions and maping of complex arguments with join (or map) can be done to simplify ansible datastructures for later use. Also have a look of dataype conversions from sets to lists, ...).


**format**: 
This simply shows the syntax for formatting i.e. numbers within a playbook

