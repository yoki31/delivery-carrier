.. _contribute:

##########
Contribute
##########

We accept with pleasure all type of contributions:

* bug reports
* pull requests
* ideas
* translations
* ...

The GitHub project is: https://github.com/OCA/carrier-delivery

********************************
Want to start with a new carrier
********************************

If you want to start using the webservice of another carrier,
you will want to extend the module `base_delivery_carrier_label`.

You can have a look at existing implementations (`PostLogistics WSBC`_,
`GLS Group - Transportation services`_).

Then you can make a pull request to add your new module in `carrier-delivery`_

.. _`PostLogistics WSBC`: https://github.com/OCA/carrier-delivery/tree/9.0/delivery_carrier_label_postlogistics
.. _`GLS Group - Transportation services`: https://github.com/OCA/carrier-delivery/tree/8.0/delivery_carrier_label_gls
.. _`E-Commerce Connector`: https://github.com/OCA/connector-ecommerce

*************************************************
Creating or maintaining a translation of this doc
*************************************************

- Install Odoo, its dependencies, sphinx, sphinx_bootstrap_theme and
  sphinx-intl
- Add `this patch
  <https://bitbucket.org/shimizukawa/sphinx-intl/pull-request/9/>`_
  to sphinx-intl (until merged) to support *fuzzy* translations
- create an empty database with the connector module installed
- ``cd delivery_carrier_label_postlogistics/doc``
- rebuild the gettext .pot source catalogs: ``make gettext``
- update the .po translation files from the latest .pot files (here for
  language 'fr'): ``sphinx-intl update -l fr -p _build/locale``
- create or edit the translation in the .po files: ``poedit
  locale/fr/LC_MESSAGES/*.po``
- compile the .po files into .mo files: ``sphinx-intl build``
- build the translated documentation to html: ``make SPHINXOPTS="-Dlanguage=fr"
  html``

XXX
The same using a `buildout
<https://bitbucket.org/anybox/public_buildbot_buildouts/src/tip/odoo-connector.cfg>`_::

    $ mkdir buildout && cd buildout
    $ wget https://bitbucket.org/anybox/public_buildbot_buildouts/raw/tip/odoo-connector.cfg -O buildout.cfg
    $ wget https://bitbucket.org/anybox/public_buildbot_buildouts/raw/tip/bootstrap.py
    $ python bootstrap.py
    $ bin/buildout
    $ createdb connectordb
    $ bin/start_openerp -d connectordb --stop-after-init
    $ cd connector/connector/doc/
    $ ../../../bin/sphinx-build -d connectordb -- -b gettext ./ _build/locale/
    $ ../../../bin/sphinx-intl -d connectordb -- update -l fr -p _build/locale/
    $ poedit locale/fr/LC_MESSAGES/*po
    $ ../../../bin/sphinx-intl -d connectordb -- build
    $ ../../../bin/sphinx-build -d connectordb -- -D language=fr -b html ./ _build/html/

Then you can see the result in _build/html/ and submit a Pull Request. Repeat the 5 last steps to update the translation if modified upstream.
