# TrapperKeeper
An SNMP trap listener

This is a simple SNMP reader that I needed recently. It's only intended to listen on the port specified and catch (and print) traps
that this port recieves. It doesn't do any responding or handling of them. V3 hasn't been tested, and the defaults in there are for
my current OS that needed it and may need to be changed for other OS's. Also note this likely will have to be run as root / admin
because it binds to a low numbered port (unless you change that setting).

It takes command line arguments of the following form:
usage: SnmpTrapperKeeper
 -f,--full-bindings       Print out the full set of bindings (not 'pretty
                          printed')
 -h,--help                Print the help message.
 -i,--listen-ip <arg>     The local IP that Trapper Keeper will listen on.
                          Default [0.0.0.0]
 -n,--listen-port <arg>   The port that Trapper Keeper will listen on.
                          Default [161]
 -p,--v3-user <arg>       The username for v3 snmp. Default [0.0.0.0]
 -T,--tcp                 Use TCP. Default [false]
 -U,--udp                 Use UDP. Default [true]
 -u,--v3-user <arg>       The username for v3 snmp. Default [0.0.0.0]
