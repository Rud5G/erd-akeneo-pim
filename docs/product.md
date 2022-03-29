

## Product Concepts

    https://api.akeneo.com/concepts/products.html

Product values should be localizable whenever you want to enrich different values among your activated locales.

Product values should be scopable whenever you want to enrich different values among your channels.


### Product values of a localizable attribute

```json
{
      "short_description": [
        {
          "locale": "en_US",
          "scope": null,
          "data": "Tshirt long sleeves"
        },
        {
          "locale": "fr_FR",
          "scope": null,
          "data": "Tshirt manches longues"
        }
      ]
    }
```


### Product values of a scopable attribute

```json
{
      "release_date": [
        {
          "locale": null,
          "scope": "ecommerce",
          "data": "2012-03-13T00:00:00+01:00"
        },
        {
          "locale": null,
          "scope": "mobile",
          "data": "2012-04-23T00:00:00+01:00"
        }
      ]
    }
```


### Product values of a localizable and scopable attribute

```json
{
      "description": [
        {
          "locale": "de_DE",
          "scope": "mobile",
          "data": "Akeneo Mug"
        },
        {
          "locale": "de_DE",
          "scope": "print",
          "data": "Akeneo Mug"
        },
        {
          "locale": "en_US",
          "scope": "mobile",
          "data": "Akeneo Mug"
        },
        {
          "locale": "en_US",
          "scope": "print",
          "data": "Akeneo Mug"
        },
        {
          "locale": "fr_FR",
          "scope": "mobile",
          "data": "Mug Akeneo"
        },
        {
          "locale": "fr_FR",
          "scope": "print",
          "data": "Mug Akeneo"
        }
      ]
    }
```


### Product value of a non localizable, non scopable attribute

```json
{
      "main_color": [
        {
          "locale": null,
          "scope": null,
          "data": "black"
        }
      ]
    }
```



{

identifier (string )  • Product identifier, i.e. the value of the only `pim_catalog_identifier` attribute

enabled (boolean , true by default) • Whether the product is enabled

family (string , null only in the case of a non variant product by default)  • Family code from which the product inherits its attributes and attributes requirements

categories (array [string] , [] by default)  • Codes of the categories in which the product is classified

groups (array [string] , [] by default)  • Codes of the groups to which the product belong

parent (string , null by default)  • Code of the parent product model when the product is a variant (only available since the 2.0). This parent can be modified since the 2.3.

values (object { attributeCode : array [ object { scope : string , locale : string , data : object , linked_data : object } ] } )  • Product attributes values, see Product values section for more details

associations (object { associationTypeCode : object { groups : array [string] , products : array [string] , product_models : array [string] } } )  • Several associations related to groups, product models and/or other products, grouped by association types

quantified_associations (object { quantifiedAssociationTypeCode : object { products : array [object] , product_models : array [object] } } )  • Several quantified associations related to products and/or product models, grouped by quantified association types (only available since the 5.0)

}
