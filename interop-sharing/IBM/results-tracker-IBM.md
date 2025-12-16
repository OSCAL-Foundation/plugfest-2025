# Result Tracker for OSCAL Compass CNCF project
OSCAL Compass project is offering Open Security Controls Assessment Language (OSCAL) content
for public review and feedback. 
Please see [content github repo](https://github.com/oscal-compass/oscal-content)

<br/>

## Interoperability Results 
The examples-direct-mapping folder contains multiple examples of the upcoming 
mapping collections OSCAL model and the related catalogs, profiles and component definitions.
https://github.com/oscal-compass/oscal-content/tree/main/examples-direct-mapping

| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| catalogs | -| - | - | - |
| profiles | -| -  | - |  |
| comp. defs.| - | -  | - |  |
| mapping| - | -  | - |  |

<br/>

<br/>

# Interoperability Results for Comply0

Web application to manage OSCAL documents. Validated against v0.1.0-preview.5 available at https://app.dev.comply0.com.
Only JSON files are accepted by the tool. Currently the version can only process JSON catalogs and profiles.  
To register for an account or request instance of the application please go to: https://www.comply0.com/


| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| catalogs/hipaa-2.0.0/catalog.json | :heavy_check_mark: | :x: | N/A | The `$.catalog.metadata.last-modified` attribute value is not a valid [`date-time-with-timezone`](https://pages.nist.gov/metaschema/specification/datatypes/#date-time-with-timezone). |
| catalogs/nist_ai_rm_gen_ai/1.0.0/catalog.json | :heavy_check_mark: | :heavy_check_mark:  | N/A | N/A |
| examples-direct-mapping/catalogs/NIST_SP-800-53_rev4/catalog.json | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| examples-direct-mapping/catalogs/PCI/catalog.json | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| examples-direct-mapping/profiles/Sample_NIST/profile.json | :heavy_check_mark: | :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| examples-direct-mapping/profiles/Sample_PCI/profile.json | :heavy_check_mark: | :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| examples-harmonized-mapping/catalogs/NIST_SP-800-53_rev4/catalog.json | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| examples-harmonized-mapping/catalogs/PCI/catalog.json | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| examples-harmonized-mapping/profiles/Harmonized_V1.0/profile.json | :heavy_check_mark: | :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| examples-harmonized-mapping/profiles/Harmonized_V1.1/profile.json | :heavy_check_mark: | :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |

<br/>