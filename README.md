## GoodRelations for PHP (GR4PHP) - A PHP API for Consuming GoodRelations E-commerce Data ##

GR4PHP is a PHP API (as library) that allows the consumption of [GoodRelations](http://purl.org/goodrelations/) data on an eligible SPARQL endpoint without requiring the developer to have a deep understanding of the underlying GoodRelations vocabulary or SPARQL queries. The API provides six abstract functions, which are interally translated into proper SPARQL queries for GoodRelations.

  * *getCompany*: Returns information about a GoodRelations **BusinessEntity**.
  * *getLocation*: Return stores in the proximity of a given geographic point.
  * *getOffers*: Returns GoodRelations **Offerings** given search criteria.
  * *getOpeningHours*: Gives opening hours to a given store (GoodRelations **LocationOfSalesOrServiceProvisioning**).
  * *getProductModel*: Returns details about model data (GoodRelations **ProductOrServiceModel**).
  * *getStore*: Gives response data to a SPARQL query searching for GoodRelations **LocationOfSalesOrServiceProvisioning**.


### Benefits of GR4PHP ###

PHP developers do not need to be fully aware of all details of GoodRelations, RDF, or SPARQL and can easily integrate GoodRelations e-commerce data, like offers, product features, or store information into their Web applications.


### Demo and Documentation ###

For demo and documentation take a look at
  * [GR4PHP testing tool](http://www.ebusiness-unibw.org/tools/gr4php/)
  * [GR4PHP documentation](http://www.ebusiness-unibw.org/tools/gr4php/doc/)


### How to start developing with GR4PHP? ###

After downloading and including the GR4PHP package into your project directory, you can pick one of the GR4PHP libary functions (see the list above). GR4PHP automatically crafts a SPARQL query for you, submits it to the configured SPARQL endpoint, fetches the results and converts them into a PHP array, on which further processing can be conducted.

The figure below sketches a flow chart of GR4PHP:

![Flow Chart of GR4PHP](http://www.ebusiness-unibw.org/tools/gr4php/images/scheme_v2.png)

### Publications ###

**Stolz, A., Ge, M. and Hepp, M.:** [GR4PHP: A Programming API for Consuming E-Commerce Data from the Semantic Web](http://www.inf.puc-rio.br/~psw12/3.pdf). Proceedings of the [First Workshop on Programming the Semantic Web (PSW 2012)](http://iswc2012.semanticweb.org/workshops/psw12.inf.puc-rio.br), in conjunction with the 11th International Semantic Web Conference (ISWC 2012) (Boston, Mass., USA, 2012). ([Slides](http://www.heppnetz.de/files/GR4PHP-ISWC2012-talk.pdf))

### Acknowledgements ###

GR4PHP is available under the terms of the GNU Lesser General Public License. The work on this project has been supported by the [German Federal Ministry of Research (BMBF)](http://www.bmbf.de/en/) by a grant under the KMU Innovativ program as part of the [Intelligent Match project](http://www.intelligent-match.de/) (FKZ 01IS10022B).

![http://www.bmbf.de/en/](http://www.productontology.org/static/bmbf.png)
