# IRI on Docker Compose

This is a repo for who want to run an IOTA Node on Docker, it's simple.

To run IRI on Docker with Docker Compose, first, download [IOTA Tangle Database](http://db.iota.partners/IOTA.partners-mainnetdb.tar.gz) into the db folder, and un-tar it.

After un-tar, you can remove that tar if you want.

Second, modify docker-compose.yml, add your Field Name and your Seed inside the file.

Additionally, if you want to manually add the neighbor to your IOTA Node, un-comment the NEIGHBORS inside iota.ini

Finally, just run `docker-compose up` and you're ready to go.

The ports used by the node are listed below, remember to adjust your firewall to let your node communicate to other node or services.
You can modify these port if you want, just remember to modify parameters too.
* 14265/tcp ( IRI API Port )
* 14777/udp ( IRI UDP Port )
* 15777/tcp ( IRI TCP Port )
* 18600/tcp ( CarrIOTA Nelson Port )
* 21310/tcp ( CarrIOTA Field Port )
* 8888/tcp ( IOTA Monitor Port )
