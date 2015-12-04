# dokku-gnatsd-plugin

## DEPRECATED
This project is now old and senile, please use [dokku-nats](http://github.com/byrnedo/dokku-nats) instead.

Simple plugin to link a single instance [gnatsd](http://nats.io/) queue to an app

## Installation

    git clone https://github.com/byrnedo/dokku-gnatsd-plugin.git /var/lib/dokku/plugins/gnatsd
    dokku plugins-install

## Commands 

    gnatsd:create                                 Creates and runs the Gnatsd container
    gnatsd:delete                                 Delete Gnatsd container
    gnatsd:info                                   Display Gnatsd container informations
    gnatsd:link <app>                             Link an <app> to the Gnatsd container
    gnatsd:logs                                   Display last logs from Gnatsd container
    gnatsd:rebuild                                Rebuild Gnatsd container
    gnatsd:unlink <app>                           Unlink an <app> from the Gnatsd container

## Example Usage

Start the gnatsd container if you haven't already

    $ dokku gnatsd:create            #server side
    $ ssh dokku@server gnatsd:create #client side

Link it to your app, say it's called `foo`:

    $ dokku gnatsd:link foo
    
or

    $ ssh dokku@server gnatsd:link foo

this will expose the following environment variables to the app `foo`:

    GNATSD_HOST
    GNATSD_PORT
    GNATSD_USERNAME
    GNATSD_PASSWORD
    GNATSD_URL
    

