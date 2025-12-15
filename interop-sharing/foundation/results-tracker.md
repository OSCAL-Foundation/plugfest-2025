# Result Tracker for OSCAL Foundation

OSCAL files provided by the OSCAL Foundation (CC0) for use in functionality and interoperability testing. This is not an exhaustive test suite, but just some simple examples.

Files are provided in JSON across the board.

#### ./edgecases/ultraminimal
The absolute most minimal OSCAL files that are still specification valid.

#### ./basic
A simple set of files to test basic tool functionality.


<br/>

# Interoperability Results for TOOLNAME

> [!NOTE]
> Copy and paste this markdown block (\<br/> to \<br/>) to add your own results!

**Short** details about the specific tool used here, provide a link for in-depth information.

Any overall notes or discussion about the content's interoperability here.

### ./edgecases/ultraminimal
| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| ultraMinimalAP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalAR.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalCatalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalComponent.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalMapping.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalPOAM.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalProfile.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalSSP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalSSP2.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |

### ./basic
| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| basicAP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicAR.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicCatalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicComponent.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicMapping.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicPOAM.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicProfile.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicSSP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicSSP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |

<br/>

<br/>

# Interoperability Results for usnistgov/oscal-cli
Tested using release 1.0.3 of the oscal-cli tool at https://github.com/usnistgov/oscal-cli

### ./edgecases/ultraminimal
| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| ultraMinimalAP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalAR.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalCatalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalComponent.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalMapping.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalPOAM.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalProfile.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalSSP.json | :heavy_check_mark:| :x: | N/A | Tool expects the "system-id" object to contain an "id", and for the "implemented-requirement" object to contain at least one "by-component" object. |
| ultraMinimalSSP2.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |

### ./basic
| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| basicAP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicAR.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicCatalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicComponent.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicMappingAtoB.json | :x: | N/A | N/A | N/A |
| basicMappingBtoA.json | :x: | N/A | N/A | N/A |
| basicPOAM.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicProfile.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicSSP.json | :heavy_check_mark:| :x: | N/A | Tool expects at least one "user" object in "system-implementation" |

<br/>

<br/>

# Interoperability Results for metaschema-framework/oscal-cli

Tested using release 2.6.0 of the oscal-cli tool at https://github.com/metaschema-framework/oscal-cli

### ./edgecases/ultraminimal
| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| ultraMinimalAP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalAR.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalCatalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalComponent.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalMapping.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalPOAM.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ultraMinimalProfile.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A | 
| ultraMinimalSSP.json | :heavy_check_mark:| :x: | N/A | Tool expects the "system-id" object to contain an "id", and for the "implemented-requirement" object to contain at least one "by-component" object. |
| ultraMinimalSSP2.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |

### ./basic
| File | Tested? | Validates? | Additonal Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| basicAP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicAR.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicCatalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicComponent.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicMappingAtoB.json | :x: | N/A | N/A | N/A |
| basicMappingBtoA.json | :x: | N/A | N/A | N/A |
| basicPOAM.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicProfile.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| basicSSP.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |

<br/>

