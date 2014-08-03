Skip entries / return from include
==================================

Ansible evaluates the "when" condition for includes on each task in the included file. So if the condition for the include becomes false during incude execution, the rest of the included script is skipped.

This way it is possible to return successfully from includes at any point.

I don't know if this is indended by the devellopers, but at least in version 1.6.3 this works.
