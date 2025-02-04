
[![Runboat](https://img.shields.io/badge/runboat-Try%20me-875A7B.png)](https://runboat.odoo-community.org/builds?repo=OCA/delivery-carrier&target_branch=14.0)
[![Pre-commit Status](https://github.com/OCA/delivery-carrier/actions/workflows/pre-commit.yml/badge.svg?branch=14.0)](https://github.com/OCA/delivery-carrier/actions/workflows/pre-commit.yml?query=branch%3A14.0)
[![Build Status](https://github.com/OCA/delivery-carrier/actions/workflows/test.yml/badge.svg?branch=14.0)](https://github.com/OCA/delivery-carrier/actions/workflows/test.yml?query=branch%3A14.0)
[![codecov](https://codecov.io/gh/OCA/delivery-carrier/branch/14.0/graph/badge.svg)](https://codecov.io/gh/OCA/delivery-carrier)
[![Translation Status](https://translation.odoo-community.org/widgets/delivery-carrier-14-0/-/svg-badge.svg)](https://translation.odoo-community.org/engage/delivery-carrier-14-0/?utm_source=widget)

<!-- /!\ do not modify above this line -->

# delivery-carrier

Repository for Delivery Carriers implementations

<!-- /!\ do not modify below this line -->

<!-- prettier-ignore-start -->

[//]: # (addons)

Available addons
----------------
addon | version | maintainers | summary
--- | --- | --- | ---
[base_delivery_carrier_files](base_delivery_carrier_files/) | 14.0.1.0.2 |  | Base module for creation of delivery carrier files
[base_delivery_carrier_label](base_delivery_carrier_label/) | 14.0.1.3.1 |  | Base module for carrier labels
[carrier_account_environment](carrier_account_environment/) | 14.0.1.0.1 | [![florian-dacosta](https://github.com/florian-dacosta.png?size=30px)](https://github.com/florian-dacosta) | Configure carriers with server_environment_files
[delivery_auto_refresh](delivery_auto_refresh/) | 14.0.1.1.4 | [![aleuffre](https://github.com/aleuffre.png?size=30px)](https://github.com/aleuffre) [![renda-dev](https://github.com/renda-dev.png?size=30px)](https://github.com/renda-dev) [![PicchiSeba](https://github.com/PicchiSeba.png?size=30px)](https://github.com/PicchiSeba) | Auto-refresh delivery price in sales orders
[delivery_carrier_agency](delivery_carrier_agency/) | 14.0.1.0.1 |  | Add a model for Carrier Agencies
[delivery_carrier_category](delivery_carrier_category/) | 14.0.1.0.0 | [![rousseldenis](https://github.com/rousseldenis.png?size=30px)](https://github.com/rousseldenis) | Adds a category to delivery carriers in order to help users classifying them
[delivery_carrier_city](delivery_carrier_city/) | 14.0.1.0.0 | [![ivantodorovich](https://github.com/ivantodorovich.png?size=30px)](https://github.com/ivantodorovich) | Integrates delivery with base_address_city
[delivery_carrier_customer_info](delivery_carrier_customer_info/) | 14.0.1.0.0 |  | Send delivery notice to the shipper from any operation.
[delivery_carrier_default_tracking_url](delivery_carrier_default_tracking_url/) | 14.0.1.0.0 | [![rousseldenis](https://github.com/rousseldenis.png?size=30px)](https://github.com/rousseldenis) | Adds the default tracking url on delivery carrier
[delivery_carrier_deposit](delivery_carrier_deposit/) | 14.0.2.0.0 |  | Create deposit slips
[delivery_carrier_info](delivery_carrier_info/) | 14.0.1.0.1 |  | Add code and description on carrier
[delivery_carrier_label_batch](delivery_carrier_label_batch/) | 14.0.1.1.1 |  | Carrier labels - Stock Batch Picking (link)
[delivery_carrier_location](delivery_carrier_location/) | 14.0.1.0.0 | [![ivantodorovich](https://github.com/ivantodorovich.png?size=30px)](https://github.com/ivantodorovich) | Integrates delivery with base_location
[delivery_carrier_multi_zip](delivery_carrier_multi_zip/) | 14.0.1.0.0 |  | Multiple ZIP intervals for the same delivery method
[delivery_carrier_package_measure_required](delivery_carrier_package_measure_required/) | 14.0.1.0.2 |  | Allow the configuration of which package measurements are required on a delivery carrier basis.
[delivery_carrier_partner](delivery_carrier_partner/) | 14.0.1.0.0 |  | Add a partner in the delivery carrier
[delivery_carrier_pricelist](delivery_carrier_pricelist/) | 14.0.1.0.2 |  | Compute method method fees based on the product's pricelist.
[delivery_carrier_return_barcode_pattern](delivery_carrier_return_barcode_pattern/) | 14.0.1.0.1 | [![mmequignon](https://github.com/mmequignon.png?size=30px)](https://github.com/mmequignon) | Allow to define a return barcode pattern on delivery methods
[delivery_correos_express](delivery_correos_express/) | 14.0.1.0.1 |  | Delivery Carrier implementation for Correos Express using their API
[delivery_cttexpress](delivery_cttexpress/) | 14.0.1.0.1 |  | Delivery Carrier implementation for CTT Express API
[delivery_free_fee_removal](delivery_free_fee_removal/) | 14.0.1.0.0 |  | Hide free fee lines on sales orders
[delivery_multi_destination](delivery_multi_destination/) | 14.0.1.1.2 |  | Multiple destinations for the same delivery method
[delivery_package_fee](delivery_package_fee/) | 14.0.1.0.3 |  | Add fees on delivered packages on shipping methods
[delivery_package_number](delivery_package_number/) | 14.0.1.2.1 |  | Set or compute number of packages for a picking
[delivery_packaging_archive](delivery_packaging_archive/) | 14.0.1.0.1 | [![mt-software-de](https://github.com/mt-software-de.png?size=30px)](https://github.com/mt-software-de) | This module allows archiving a delivery packaging
[delivery_postlogistics](delivery_postlogistics/) | 14.0.1.1.0 |  | Print PostLogistics shipping labels using the Barcode web service
[delivery_postlogistics_dangerous_goods](delivery_postlogistics_dangerous_goods/) | 14.0.1.0.0 |  | Declare dangerous goods when generating postlogistics labels
[delivery_postlogistics_server_env](delivery_postlogistics_server_env/) | 14.0.1.0.0 |  | Server Environment layer for Delivery Postlogistics
[delivery_price_collection_cost](delivery_price_collection_cost/) | 14.0.1.0.0 |  | Add delivery collection costs as a separate line in the SO
[delivery_price_collection_cost_product_domain](delivery_price_collection_cost_product_domain/) | 14.0.1.0.1 |  | Bridge module between Delivery Collection Cost and Product Domain
[delivery_price_method](delivery_price_method/) | 14.0.1.0.1 |  | Provides fields to be able to contemplate the tracking statesand also adds a global fields
[delivery_price_product_domain](delivery_price_product_domain/) | 14.0.1.0.4 | [![solo4games](https://github.com/solo4games.png?size=30px)](https://github.com/solo4games) [![CetmixGitDrone](https://github.com/CetmixGitDrone.png?size=30px)](https://github.com/CetmixGitDrone) | Apply domain to product in shipping charges rules
[delivery_price_rule_untaxed](delivery_price_rule_untaxed/) | 14.0.1.0.3 | [![AshishHirapara](https://github.com/AshishHirapara.png?size=30px)](https://github.com/AshishHirapara) | Add untaxed amount to variables for price delivery price rule
[delivery_purchase](delivery_purchase/) | 14.0.1.3.0 |  | Delivery costs in purchases
[delivery_roulier](delivery_roulier/) | 14.0.1.1.0 | [![florian-dacosta](https://github.com/florian-dacosta.png?size=30px)](https://github.com/florian-dacosta) | Integration of multiple carriers
[delivery_roulier_chronopost_fr](delivery_roulier_chronopost_fr/) | 14.0.1.0.1 |  | Delivery Chronopost France
[delivery_roulier_laposte_fr](delivery_roulier_laposte_fr/) | 14.0.1.2.0 | [![florian-dacosta](https://github.com/florian-dacosta.png?size=30px)](https://github.com/florian-dacosta) | Generate Label for La Poste/Colissimo
[delivery_roulier_option](delivery_roulier_option/) | 14.0.1.0.0 | [![florian-dacosta](https://github.com/florian-dacosta.png?size=30px)](https://github.com/florian-dacosta) | Add options to roulier modules
[delivery_schenker](delivery_schenker/) | 14.0.2.0.1 |  | Delivery Carrier implementation for DB Schenker API
[delivery_schenker_picking_volume](delivery_schenker_picking_volume/) | 14.0.1.2.0 |  | Glue module between delivery_schenker and stock_picking_volumeWith this module the transmitted volume is changed,it uses the computed volume from stock_picking_volume
[delivery_schenker_quant_package_dimension](delivery_schenker_quant_package_dimension/) | 14.0.2.0.1 | [![mt-software-de](https://github.com/mt-software-de.png?size=30px)](https://github.com/mt-software-de) | Glue module between delivery_schenker and stock_quant_package_dimensionWith this module the transmitted package volume is changed,it uses the computed volume from stock_quant_package_dimension.Also the dimensions length, width and height of a package getting added to the request
[delivery_send_to_shipper_at_operation](delivery_send_to_shipper_at_operation/) | 14.0.1.0.2 |  | Send delivery notice to the shipper from any operation.
[delivery_state](delivery_state/) | 14.0.1.1.2 |  | Provides fields to be able to contemplate the tracking statesand also adds a global fields
[delivery_tnt_oca](delivery_tnt_oca/) | 14.0.1.2.5 | [![victoralmau](https://github.com/victoralmau.png?size=30px)](https://github.com/victoralmau) | Integrate TNT webservice
[delivery_ups_oca](delivery_ups_oca/) | 14.0.1.0.1 |  | Integrate UPS webservice
[partner_default_delivery_carrier](partner_default_delivery_carrier/) | 14.0.1.0.0 | [![SilvioC2C](https://github.com/SilvioC2C.png?size=30px)](https://github.com/SilvioC2C) | Allows defining default delivery methods for partners
[partner_delivery_zone](partner_delivery_zone/) | 14.0.1.1.1 |  | Set on partners a zone for delivery goods
[server_environment_delivery](server_environment_delivery/) | 14.0.1.0.0 |  | Configure prod environment for delivery carriers
[stock_picking_carrier_from_rule](stock_picking_carrier_from_rule/) | 14.0.1.0.0 |  | Set the carrier on picking if the stock rule used has a partner address set with a delivery method.
[stock_picking_delivery_link](stock_picking_delivery_link/) | 14.0.1.0.0 |  | Adds link to the delivery on all intermediate operations.

[//]: # (end addons)

<!-- prettier-ignore-end -->

## Licenses

This repository is licensed under [AGPL-3.0](LICENSE).

However, each module can have a totally different license, as long as they adhere to Odoo Community Association (OCA)
policy. Consult each module's `__manifest__.py` file, which contains a `license` key
that explains its license.

----
OCA, or the [Odoo Community Association](http://odoo-community.org/), is a nonprofit
organization whose mission is to support the collaborative development of Odoo features
and promote its widespread use.
