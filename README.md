# dokku-gnatsd-plugin

[![Join the chat at https://gitter.im/byrnedo/dokku-gnatsd-plugin](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/byrnedo/dokku-gnatsd-plugin?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

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

