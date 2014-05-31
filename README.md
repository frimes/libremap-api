# LibreMap

LibreMap is a **scalable**, **global** and **decentralized** router database and map visualization for community networks, such as guifi, Altermundi, FunkFeuer, ninux, freifunk, Commotion... It emerged around the [is4cwn](http://2013.wirelesssummit.org/) by merging the maps of [AlterMap](https://colectivo.altermundi.net/projects/altermap) (Altermundi) and [OpenWiFiMap](https://github.com/freifunk/openwifimap-html5) (freifunk).

LibreMap consists of 2 main parts:
* **[libremap-webui](https://github.com/libremap/libremap-webui):** the HTML5 web app, see [libremap.net](http://libremap.net).
* **libremap-api (this repo!):** the CouchDB server design document that exposes the *LibreMap API*.

## Goals of LibreMap:
* show the state of all community networks, both on a global and local scale.
* decentralized.
* easy to use and extend.
* independent of involved routing protocols and other technical details.
* scale up to global level (>100k routers).
* share open data for community networks.

There's a presentation ([slides](http://libre-mesh.github.io/libremap-talk-2013-is4cwn/)) from the [is4cwn](http://2013.wirelesssummit.org/) that explains the concept and some details.

## Under the hood
* Built with [CouchDB](http://couchdb.apache.org) and [GeoCouch](https://github.com/couchbase/geocouch/).
* HTTP REST API.
* Decentralized/federated with CouchDB's built-in replication.
* Each community can set up its own LibreMap instance (see the [install docs](doc-install.md)) and let it replicate to/from existing instances (see the list of [LibreMap instances](libremap-instances.json)). The replication may look like this:
![Replication illustration](http://libre-mesh.github.io/libremap-talk-2013-is4cwn/images/replication.svg)


## Join the LibreMap network!
If you're interested in setting up an LibreMap instance, then head over to the [docs](#documentation) and don't be shy if you have questions -- [get in touch](#contact) with us!. When your instance is up and running, please include it in the [libremap-instances.json](libremap-instances.json) file of this repo.

## Documentation
* [Installation and replication](doc-install.md)
* [API documentation](doc-api.md)

## Bugs and feature requests
Please use the issues tracker if you found a bug or have an idea how to improve LibreMap!

## Contact
LibreMap is maintained by [André](https://github.com/andrenarchy) and [Nico](https://github.com/nicoechaniz). There is a **[mailing list](http://lists.libremap.net/mailman/listinfo/discussion)** for questions and discussions about LibreMap, so feel free to drop a line there!

## License

LibreMap is licensed under [GPL3](LICENSE).
