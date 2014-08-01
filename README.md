Ansible playground
==================

This is a place for collected ansible stuff I expremimented with during learning how to write playbooks. Might be interesting - at least for me to remember ;)


List of plays
-------------

**link_or_override**: 
Link files from source to dest or use local overrides.

This makes use of filtersfor handling of unions/differences of lists, set_fact for variable registration and opened my eyes on use of complex datatypes: Ansible parses all variables with jinja2 (python expressions like split() - even on filter expressions, maping of complex arguments with join, have a look of dataype conversions from sets to lists, ...).
