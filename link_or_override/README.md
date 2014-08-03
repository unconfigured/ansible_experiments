Link files or use local template if available
=============================================

This playbooks takes a module and extension list to build up a filelist. Each files availability in sourcedir is checked and if the file is available it gets linked to destdir except there is a local override/template on the mgmt host. In this case the template is copied. 

All actions, like adding/removing modules/overrides after initial setup is handled and the target dir will be changed accordingly. Files which are no more existing in sourcedir will get cleaned up.

 
This playbook makes no changes on the target, except if really nessessary!


Usecase:
--------
This module can be used in apache setups, where modules.(load|conf) from modules.available get linked to modules.active. In case you want to have a config override on the mgmt host which should be templated instead of taken from modules.activated, the template will be used.

