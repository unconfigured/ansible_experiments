Reverse connect
===============

This shows a way to carry a port from you management host to the client which you are currently manageing. For example to gain git or webserver access only for the management session. 

The disadvantage is, that the port is available for a fixed time configured in the playbook but at least you cannot forget to remove access to ther service. Another advantage is, you can bind you webserver to localhost to be sure nobody cann access it even when stuff like firewalling fails.

Another way would be to do ssh connection with port forwarding as "local_action" and put the command as remote action for the ssh call. But with the way shown here you can keep things seperate, use the port multiple times without reconnecting and use all ansible modules as usual.

Site note: when using raw mode and disable facts gathering during startup, you can install python from your forwarded packet repository
