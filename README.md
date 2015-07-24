# dokku-gnatsd-plugin

Simple plugin to link a gnatsd queue to an app

## Installation

    https://github.com/byrnedo/dokku-gnatsd-plugin.git /var/lib/dokku/plugins/gnatsd
    dokku plugins-install

## Commands 

    gnatsd:delete                                 Delete Gnatsd container
    gnatsd:info                                   Display Gnatsd container informations
    gnatsd:link <app>                             Link an <app> to the Gnatsd container
    gnatsd:logs                                   Display last logs from Gnatsd container
    gnatsd:rebuild                                Rebuild Gnatsd container (keep persistend data)
    gnatsd:start                                  Starts the Gnatsd container
    gnatsd:unlink <app>                           Unlink an <app> from the Gnatsd container

