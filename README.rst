Inspired by https://github.com/fschulze/devpi-buildout

Setup
=====

bin/supervisord
bin/devpi use http://localhost:3141/
bin/devpi login root --password=
bin/devpi user -c plone password=plone
bin/devpi login plone --password=plone
bin/devpi index -c prod
bin/devpi index -c 5.0 bases=plone/prod
bin/devpi index -c 4.3 bases=plone/prod
