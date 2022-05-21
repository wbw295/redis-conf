
cluster help

```
192.168.182.131:7031> cluster help
 1) CLUSTER <subcommand> [<arg> [value] [opt] ...]. Subcommands are:
 2) ADDSLOTS <slot> [<slot> ...]
 3)     Assign slots to current node.
 4) ADDSLOTSRANGE <start slot> <end slot> [<start slot> <end slot> ...]
 5)     Assign slots which are between <start-slot> and <end-slot> to current node.
 6) BUMPEPOCH
 7)     Advance the cluster config epoch.
 8) COUNT-FAILURE-REPORTS <node-id>
 9)     Return number of failure reports for <node-id>.
10) COUNTKEYSINSLOT <slot>
11)     Return the number of keys in <slot>.
12) DELSLOTS <slot> [<slot> ...]
13)     Delete slots information from current node.
14) DELSLOTSRANGE <start slot> <end slot> [<start slot> <end slot> ...]
15)     Delete slots information which are between <start-slot> and <end-slot> from current node.
16) FAILOVER [FORCE|TAKEOVER]
17)     Promote current replica node to being a master.
18) FORGET <node-id>
19)     Remove a node from the cluster.
20) GETKEYSINSLOT <slot> <count>
21)     Return key names stored by current node in a slot.
22) FLUSHSLOTS
23)     Delete current node own slots information.
24) INFO
25)     Return information about the cluster.
26) KEYSLOT <key>
27)     Return the hash slot for <key>.
28) MEET <ip> <port> [<bus-port>]
29)     Connect nodes into a working cluster.
30) MYID
31)     Return the node id.
32) NODES
33)     Return cluster configuration seen by node. Output format:
34)     <id> <ip:port> <flags> <master> <pings> <pongs> <epoch> <link> <slot> ...
35) REPLICATE <node-id>
36)     Configure current node as replica to <node-id>.
37) RESET [HARD|SOFT]
38)     Reset current node (default: soft).
39) SET-CONFIG-EPOCH <epoch>
40)     Set config epoch of current node.
41) SETSLOT <slot> (IMPORTING <node-id>|MIGRATING <node-id>|STABLE|NODE <node-id>)
42)     Set slot state.
43) REPLICAS <node-id>
44)     Return <node-id> replicas.
45) SAVECONFIG
46)     Force saving cluster configuration on disk.
47) SLOTS
48)     Return information about slots range mappings. Each range is made of:
49)     start, end, master and replicas IP addresses, ports and ids
50) SHARDS
51)     Return information about slot range mappings and the nodes associated with them.
52) LINKS
53)     Return information about all network links between this node and its peers.
54)     Output format is an array where each array element is a map containing attributes of a link
55) HELP
56)     Prints this help.
```