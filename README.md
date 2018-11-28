# graph

Copied "Digital Clock" code in order to set up my environment correctly.

## Build

You need qmake and make installed

First, run 

```sh
qmake -makefile
qmake
make
```

This should make the `graph` binary file appear in your current folder.

Then upload that bin file to your remarkable at /usr/bin/graph

### Draft

If you're using the draft launcher, upload the draft-loader file to /etc/draft/XX-graph, where XX is whatever number you want.
draft programs are listed in alphabetical order, so the higher the number you pick, the later it will appear in the list.

You'll have to restart your remarkable to get your loader to show in the listings.

### Non Draft

To run the program, you'll have to ssh into your remarkable and run

```sh
systemctl stop xochitl
graph
```

To restart xochitl (The main remarkable ui), just run

```sh
systemctl start xochitl
```