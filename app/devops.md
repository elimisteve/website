---
layout: page
---

## Developper

### Package your software!

To package your software, and invite all existing IndieHosters to start offering hosting for it, the easiest way is to create a Dockerfile that can either run multiple domains, or that can run behind an SNI offloader.

Make sure to expose all folders that will contain mutable data as Docker volumes.

If there is a database, make sure to provide a dump script which needs to be run before each snapshot of the exposed volumes, and to import the database from that dump on startup (and then don't expose the database binary data folder as a volume).

If it's a lamp application, then you can take [Michiel's WordPress container](https://github.com/indiehosters/dockerfiles/tree/master/per-user/wordpress) as a starting point.

If the application cannot run inside a container, then just provide install instructions for VMs.

Once you've done this, you can create a pull request on https://github.com/indiehosters/website, and this will also alert all existing IndieHosters who may want to start offering hosting for your software.

## SysAdmin

### Join the IndieHosters network!

To become an IndieHosters, you need to offer at least one of our products. If you do, then we'll add you to the list!

### References

{% for reference in site.references %}
#### {{ reference.title }}

{{ reference.output }}
{% endfor %}

