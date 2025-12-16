# Result Tracker for NIST Examples and NIST OSCAL Content

These files originate from NIST's [OSCAL Content Repository](https://github.com/usnistgov/oscal-content) and are provided here freely under their CC0 license. 

> [!NOTE]
> Format is purposefully left unspecified to reduce tracker complexity. Please include which formats your tool ingested at the top of your results!

#### ./nist.gov
This folder includes OSCAL versions of various NIST catalogs and profiles - including SP 800-53, SP 800-171, and the Cybersecurity Framework.

#### ./examples
This folder includes various basic examples of OSCAL documents created during OSCAL's development.

<br/>

### Quick links to participating tools
[Results Template](https://github.com/OSCAL-Foundation/plugfest-2025/blob/main/interop-sharing/nist/results-tracker.md#interoperability-results-for-toolname)

[NIST OSCAL-CLI](https://github.com/OSCAL-Foundation/plugfest-2025/blob/main/interop-sharing/nist/results-tracker.md#interoperability-results-for-nist-oscal-cli)

[Metaschema Framework OSCAL-CLI](https://github.com/OSCAL-Foundation/plugfest-2025/blob/main/interop-sharing/nist/results-tracker.md#interoperability-results-for-metaschema-frameworkoscal-cli)




<br/>

# Interoperability Results for NIST OSCAL-CLI 

Tested using release 1.0.3 of the oscal-cli tool at https://github.com/usnistgov/oscal-cli

All files tested using JSON versions.

### ./nist.gov
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| SP 800-53r4 Catalog | :heavy_check_mark: | :x: | N/A | Errors regarding use of deprecated fields. |
| SP 800-53r4 Profiles | :heavy_check_mark: | :x: | Resolved profiles validate?::x: | [/profile/modify[1]/alter[1]/add[1]/prop[1]/@name] Value 'priority' doesn't match one of 'alt-identifier, label, marking, or sort-id' at path '/profile/modify[1]/alter[1]/add[1]/prop[1]/@name'|
| SP 800-53r5 Catalog | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| SP 800-53r5 Profiles | :heavy_check_mark: | :heavy_check_mark: | Resolved profiles validate?::heavy_check_mark: | N/A |
| CSF Catalog | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| SP 800-171r3 | :heavy_check_mark: | :x: | N/A | Numerous errors on regarding label strings pattern mismatches. #/catalog/groups/0: extraneous key [controls] is not permitted |
| SP 800-218v1 | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |


### ./examples
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| catalog/*/basic-catalog.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| profile/*/basic-profile.\* | :heavy_check_mark:| :heavy_check_mark: | Resolved profile validates?::x: | Same error on freshly resolved profile as below. |
| profile/*/basic-profile-resolved.\* | :heavy_check_mark:| :x: | N/A | Value 'item' doesn't match one of 'assessment-objective or objective' at path '/catalog/control[1]/part[3]/part[4]/@name' |
| ssp/*/ssp-example.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| component-definition/*/example-component-definition.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ssp/*/ifa_ssp.\* | :heavy_check_mark: | :heavy_check_mark:| N/A | N/A |
| ap/*/ifa_assessment-plan.\* | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| ar/*/ifa_assessment-results.\* | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| poam/*/ifa_plan-of-action-and-milestones.\* | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |

<br/>



<br/>

# Interoperability Results for metaschema-framework/oscal-cli

Tested using release 2.6.0 of the oscal-cli tool at https://github.com/metaschema-framework/oscal-cli

All files tested using JSON versions.

### ./nist.gov
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| SP 800-53r4 Catalog | :heavy_check_mark: | :x: | N/A | Errors regarding use of deprecated fields. [ERROR] [/catalog/group[12]/control[5]/link[2]] oscal-unique-link-in-context-location: Unique constraint violation at paths '/catalog/group[12]/control[5]/link[1]' and '/catalog/group[12]/control[5]/link[2]'|
| SP 800-53r4 Profiles | :heavy_check_mark: | :x: | Resolved profiles validate?::x: | [/profile/modify[1]/alter[1]/add[1]/prop[1]/@name] Value 'priority' doesn't match one of 'alt-identifier, label, marking, or sort-id' at path '/profile/modify[1]/alter[1]/add[1]/prop[1]/@name'|
| SP 800-53r5 Catalog | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| SP 800-53r5 Profiles | :heavy_check_mark: | :heavy_check_mark: | Resolved profiles validate?::heavy_check_mark: | N/A |
| CSF Catalog | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| SP 800-171r3 | :heavy_check_mark: | :x: | N/A | Numerous errors on regarding label strings pattern mismatches. #/catalog/groups/0: extraneous key [controls] is not permitted |
| SP 800-218v1 | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |


### ./examples
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| catalog/*/basic-catalog.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| profile/*/basic-profile.\* | :heavy_check_mark:| :heavy_check_mark: | Resolved profile validates?::x: | Same error on freshly resolved profile as below. |
| profile/*/basic-profile-resolved.\* | :heavy_check_mark:| :x: | N/A | [ERROR] [/catalog/control[1]/part[3]/part[4]/@name] oscal-control-statement-part-name: Value 'item' doesn't match one of 'assessment-objective or objective' at path '/catalog/control[1]/part[3]/part[4]/@name' |
| ssp/*/ssp-example.\* | :heavy_check_mark:| :x: | N/A | FODC0002: An error occurred while evaluating the expression 'resolve-profile(doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-profile/@href))))/catalog': Unable to retrieve the resource identified by the URI 'https://github.com/usnistgov/oscal-content/archive/refs/tags/v1.3.0.zip'. |
| component-definition/*/example-component-definition.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ssp/*/ifa_ssp.\* | :heavy_check_mark: | :x:| N/A | FODC0002: An error occurred while evaluating the expression 'resolve-profile(doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-profile/@href))))/catalog': Unable to retrieve the resource identified by the URI 'https://github.com/usnistgov/oscal-content/archive/refs/tags/v1.3.0.zip'. |
| ap/*/ifa_assessment-plan.\* | :heavy_check_mark: | :x: | N/A | FODC0002: An error occurred while evaluating the expression 'recurse-depth('.[import-ssp]/doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-ssp/@href)))/system-security-plan|.[import-profile]/resolve-profile(doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-profile/@href))))/catalog')': Unable to retrieve the resource identified by the URI 'https://github.com/usnistgov/oscal-content/archive/refs/tags/v1.3.0.zip'. |
| ar/*/ifa_assessment-results.\* | :heavy_check_mark: | :x: | N/A | FODC0002: An error occurred while evaluating the expression 'recurse-depth('.[import-ap]/doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-ap/@href)))/assessment-plan|.[import-ssp]/doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-ssp/@href)))/system-security-plan|.[import-profile]/resolve-profile(doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-profile/@href))))/catalog')': Unable to retrieve the resource identified by the URI 'https://github.com/usnistgov/oscal-content/archive/refs/tags/v1.3.0.zip'. |
| poam/*/ifa_plan-of-action-and-milestones.\* | :heavy_check_mark: | :x: | N/A | FODC0002: An error occurred while evaluating the expression 'recurse-depth('.[import-ap]/doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-ap/@href)))/assessment-plan|.[import-ssp]/doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-ssp/@href)))/system-security-plan|.[import-profile]/resolve-profile(doc(resolve-uri(Q{http://csrc.nist.gov/ns/oscal/1.0}resolve-reference(import-profile/@href))))/catalog')': Unable to retrieve the resource identified by the URI 'https://github.com/usnistgov/oscal-content/archive/refs/tags/v1.3.0.zip'. |

<br/>

<br />

# Interoperability Results for Comply0

Web application to manage OSCAL documents. Validated against v0.1.0-preview.5 available at https://app.dev.comply0.com.
Only JSON files are accepted by the tool. Currently the version can only process JSON catalogs and profiles.  
To register for an account or request instance of the application please go to: https://www.comply0.com/

### ./nist.gov
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| csf/v2.0/json/NIST_CSF_v2.0_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev4/v2.0/json/NIST_SP-800-53_rev4_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev4/v2.0/json/NIST_SP-800-53_rev4_HIGH-baseline-resolved-profile_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev4/v2.0/json/NIST_SP-800-53_rev4_LOW-baseline-resolved-profile_catalog.json.json | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| SP800-53/rev4/v2.0/json/NIST_SP-800-53_rev4_MODERATE-baseline-resolved-profile_catalog.json.json | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| SP800-53/rev4/v2.0/json/NIST_SP-800-53_rev4_HIGH-baseline_profile.json | :heavy_check_mark:| :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| SP800-53/rev4/v2.0/json/NIST_SP-800-53_rev4_LOW-baseline_profile.json.json | :heavy_check_mark: | :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| SP800-53/rev4/v2.0/json/NIST_SP-800-53_rev4_MODERATE-baseline_profile.json.json | :heavy_check_mark: | :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_HIGH-baseline-resolved-profile_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_LOW-baseline-resolved-profile_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_MODERATE-baseline-resolved-profile_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_PRIVACY-baseline-resolved-profile_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_HIGH-baseline_profile.json | :heavy_check_mark:| :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_LOW-baseline_profile.json | :heavy_check_mark:| :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_MODERATE-baseline_profile.json | :heavy_check_mark:| :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| SP800-53/rev5/v2.0/json/NIST_SP-800-53_rev5_PRIVACY_profile.json | :heavy_check_mark:| :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| SP800-171/rev3/json/NIST_SP800-171_rev3_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP800-218/ver1/json/NIST_SP800-218_ver1_catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |


### ./examples
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| catalog/json/basic-catalog.json | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| profile/json/basic-profile.json | :heavy_check_mark:| :heavy_check_mark: | Referenced catalog needs to be uploaded to the web application separately and `$.profile.imports.href` needs to be fixed up. | N/A |
| profile/json/basic-profile-resolved.json | :heavy_check_mark: | :heavy_check_mark: | Treated as a catalog. | N/A  |

<br />

<br />

# Interoperability Results for TOOLNAME

> [!NOTE]
> Copy and paste this markdown block (\<br/> to \<br/>) then delete this note to add your own results!

**Short** details about the specific tool used here, provide a link for in-depth information.

Any overall notes or discussion about the content's interoperability here.

### ./nist.gov
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| SP 800-53r4 Catalog | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| SP 800-53r4 Profiles | :heavy_check_mark: | :heavy_check_mark: | Resolved profiles validate?::heavy_check_mark: | N/A |
| SP 800-53r5 Catalog | :heavy_check_mark: | :heavy_check_mark: | N/A | N/A |
| SP 800-53r5 Profiles | :heavy_check_mark: | :heavy_check_mark: | Resolved profiles validate?::heavy_check_mark: | N/A |
| CSF Catalog | :x: | N/A | N/A | N/A |
| SP 800-171r3 | :x: | N/A | N/A | N/A |
| SP 800-218v1 | :x: | N/A | N/A | N/A |


### ./examples
| File | Tested? | Validates? | Additional Execution/Processing Results | Notes/Errors |
|------|---------|------------|------------------------------|-------------|
| catalog/*/basic-catalog.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| profile/*/basic-profile.\* | :heavy_check_mark:| :heavy_check_mark: | Resolved profile validates?::heavy_check_mark: | N/A |
| profile/*/basic-profile-resolved.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ssp/*/ssp-example.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| component-definition/*/example-component-definition.\* | :heavy_check_mark:| :heavy_check_mark: | N/A | N/A |
| ssp/*/ifa_ssp.\* | :x: | N/A | N/A | N/A |
| ap/*/ifa_assessment-plan.\* | :x: | N/A | N/A | N/A |
| ar/*/ifa_assessment-results.\* | :x: | N/A | N/A | N/A |
| poam/*/ifa_plan-of-action-and-milestones.\* | :x: | N/A | N/A | N/A |

<br/>

