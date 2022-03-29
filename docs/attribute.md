






Below is the list of attribute types and their description:

| Attribute | Attribute type | Description |
| --------------- | --------------- | --------------- |
| Identifier | pim_catalog_identifier | a code to identify your product, this code must be unique. It can be a SKU, a MPN... This attribute is mandatory to create products. |
| Text | pim_catalog_text | a single-line text field that can contain up to 255 characters, it is usually used for a product name. |
| Text area | pim_catalog_textarea | a multi-line text field that can be used for a product description. |
| Simple select | pim_catalog_simpleselect | a single-choice list coming with custom options. Only one value can be selected among the available options. |
| Multi select | pim_catalog_multiselect | a multi-choice list coming with custom options. More than one value can be selected amongst the available options. |
| Yes/No | pim_catalog_boolean | a boolean attribute |
| Date | pim_catalog_date | a date field, the PIM will display a calendar to choose the date, which includes day, month and year. |
| Number | pim_catalog_number | a single-line field that can only contain digits. |
| Measurement | pim_catalog_metric | a single-line field composed of a first field containing a value and a second field containing a measurement unit. It allows you to automatically convert measurement values to others to fit your export needs. |
| Price | pim_catalog_price_collection | a price attribute with values per currency. The displayed values will depend on the currencies enabled in the PIM. |
| Image | pim_catalog_image | a drag and drop down zone to upload an image (extensions allowed: gif, jfif, jif, jpeg, jpg, pdf, png, psd, tif, tiff) |
| File | pim_catalog_file | a drag and drop down zone to upload a file (allowed extensions: csv, doc, docx, mp3, pdf) |
| Asset collection (Enterprise Edition only) | pim_catalog_asset_collection | an advanced attribute type to manage several digital resources like pictures, pdf files, Youtube videos... |
| Reference entity single link (Enterprise Edition only) | akeneo_reference_entity | allows enriching common data related to products with a rich content (text, images...), more complex than just a code and labels. |
| Reference entity multiple links (Enterprise Edition only) | akeneo_reference_entity_collection | the same as above but allowing you to manage multiple links |
| Reference data simple select | pim_reference_data_simpleselect | allows you to manage any kind of data that has its own properties, as a single-choice select. |
| Reference data multi select | pim_reference_data_multiselect | allows you to manage any kind of data that has its own properties, as a multi-choice select. |
| Table (Growth and Enterprise editions only) | pim_catalog_table | allows you to manage multidimensional data in the form of a table |


