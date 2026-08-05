## @hdruk/gateway-api-sdk@0.0.0-test5

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install @hdruk/gateway-api-sdk@0.0.0-test5 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AdminDataCustodianNetworksApi* | [**fetchAdminDataCustodianNetworks**](docs/AdminDataCustodianNetworksApi.md#fetchadmindatacustodiannetworks) | **GET** /api/v2/admin/data_custodian_networks | DataCustodianNetworks@adminIndex
*AdminSearchApi* | [**createAdminSearchReindex**](docs/AdminSearchApi.md#createadminsearchreindex) | **POST** /api/v1/admin/search/reindex | Queue a drop+recreate+import of a search entity\&#39;s Typesense collection
*AdminSearchApi* | [**fetchAdminSearchStatus**](docs/AdminSearchApi.md#fetchadminsearchstatus) | **GET** /api/v1/admin/search/status | Get Typesense collection status for every onboarded search entity
*AdminSearchApi* | [**updateAdminSearchFeature**](docs/AdminSearchApi.md#updateadminsearchfeature) | **POST** /api/v1/admin/search/feature | Activate or deactivate a search-related Pennant feature flag
*ApplicationApi* | [**createApplications**](docs/ApplicationApi.md#createapplications) | **POST** /api/v1/applications | ApplicationController@store
*ApplicationApi* | [**deleteApplications**](docs/ApplicationApi.md#deleteapplications) | **DELETE** /api/v1/applications/{id} | ApplicationController@delete
*ApplicationApi* | [**editApplications**](docs/ApplicationApi.md#editapplications) | **PATCH** /api/v1/applications/{id} | ApplicationController@edit
*ApplicationApi* | [**fetchAllApplications**](docs/ApplicationApi.md#fetchallapplications) | **GET** /api/v1/applications | ApplicationController@index
*ApplicationApi* | [**fetchAllSitemap**](docs/ApplicationApi.md#fetchallsitemap) | **GET** /api/v1/sitemap | SiteMapController@index
*ApplicationApi* | [**fetchApplications**](docs/ApplicationApi.md#fetchapplications) | **GET** /api/v1/applications/{id} | ApplicationController@show
*ApplicationApi* | [**patchApplicationsClientId**](docs/ApplicationApi.md#patchapplicationsclientid) | **PATCH** /api/v1/applications/{id}/clientid | ApplicationController@generateClientIdById
*ApplicationApi* | [**updateApplications**](docs/ApplicationApi.md#updateapplications) | **PUT** /api/v1/applications/{id} | ApplicationController@update
*AuthenticationApi* | [**authentication**](docs/AuthenticationApi.md#authentication) | **POST** /api/v1/auth | AuthController@checkAuthorization
*AuthenticationApi* | [**login**](docs/AuthenticationApi.md#login) | **POST** /api/v1/auth/login | AuthController@login
*AuthenticationApi* | [**register**](docs/AuthenticationApi.md#register) | **POST** /api/v1/auth/register | AuthController@register
*CancerTypeFilterApi* | [**getCancerTypeFilter**](docs/CancerTypeFilterApi.md#getcancertypefilter) | **GET** /api/v1/cancer-type-filters/{filter_id} | Get a single cancer type filter
*CancerTypeFilterApi* | [**getCancerTypeFilters**](docs/CancerTypeFilterApi.md#getcancertypefilters) | **GET** /api/v1/cancer-type-filters | Get all cancer type filters
*CollectionsApi* | [**countUniqueFieldsCollections**](docs/CollectionsApi.md#countuniquefieldscollections) | **GET** /api/v1/collections/count/{field} | CollectionController@count
*CollectionsApi* | [**countUniqueFieldsCollectionsV2**](docs/CollectionsApi.md#countuniquefieldscollectionsv2) | **GET** /api/v2/collections/count/{field} | CollectionController@count
*CollectionsApi* | [**createCollections**](docs/CollectionsApi.md#createcollections) | **POST** /api/v2/collections | CollectionController@store
*CollectionsApi* | [**deleteCollectionsV2**](docs/CollectionsApi.md#deletecollectionsv2) | **DELETE** /api/v2/collections/{id} | Delete a collection
*CollectionsApi* | [**editCollectionsV2**](docs/CollectionsApi.md#editcollectionsv2) | **PATCH** /api/v2/collections/{id} | Edit a collection
*CollectionsApi* | [**fetchAllCollections**](docs/CollectionsApi.md#fetchallcollections) | **GET** /api/v1/collections | CollectionController@index
*CollectionsApi* | [**fetchAllCollectionsV2**](docs/CollectionsApi.md#fetchallcollectionsv2) | **GET** /api/v2/collections | CollectionController@index
*CollectionsApi* | [**fetchCollections**](docs/CollectionsApi.md#fetchcollections) | **GET** /api/v1/collections/{id} | CollectionController@show
*CollectionsApi* | [**fetchCollectionsV2**](docs/CollectionsApi.md#fetchcollectionsv2) | **GET** /api/v2/collections/{id} | CollectionController@show
*CollectionsApi* | [**updateCollectionsV2**](docs/CollectionsApi.md#updatecollectionsv2) | **PUT** /api/v2/collections/{id} | Update a collection
*CustomerSatisfactionApi* | [**createCsat**](docs/CustomerSatisfactionApi.md#createcsat) | **POST** /api/v1/csat | Create Customer Satisfaction Score
*CustomerSatisfactionApi* | [**editCsat**](docs/CustomerSatisfactionApi.md#editcsat) | **PATCH** /api/v1/csat/{id} | Update Customer Satisfaction Description
*DarIntegrationApi* | [**createDarIntegration**](docs/DarIntegrationApi.md#createdarintegration) | **POST** /api/v1/dar-integration/{id} | DarIntegration@store
*DarIntegrationApi* | [**deleteDarIntegration**](docs/DarIntegrationApi.md#deletedarintegration) | **DELETE** /api/v1/dar-integrations/{id} | DarIntegration@destroy
*DarIntegrationApi* | [**editDarIntegration**](docs/DarIntegrationApi.md#editdarintegration) | **PATCH** /api/v1/dar-integration/{id} | DarIntegration@edit
*DarIntegrationApi* | [**fetchAllDarIntegrations**](docs/DarIntegrationApi.md#fetchalldarintegrations) | **GET** /api/v1/dar-integration | DarIntegration@index
*DarIntegrationApi* | [**fetchDarIntegration**](docs/DarIntegrationApi.md#fetchdarintegration) | **GET** /api/v1/dar-integration/{id} | DarIntegration@show
*DarIntegrationApi* | [**updateDarIntegration**](docs/DarIntegrationApi.md#updatedarintegration) | **PUT** /api/v1/dar-integration/{id} | DarIntegration@update
*DataAccessApplicationApi* | [**deleteDarApplicationFiles**](docs/DataAccessApplicationApi.md#deletedarapplicationfiles) | **DELETE** /api/v1/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
*DataAccessApplicationApi* | [**deleteDarApplications**](docs/DataAccessApplicationApi.md#deletedarapplications) | **DELETE** /api/v1/dar/applications/{id} | DataAccessApplication@destroy
*DataAccessApplicationApi* | [**deleteTeamDarApplicationFile**](docs/DataAccessApplicationApi.md#deleteteamdarapplicationfile) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
*DataAccessApplicationApi* | [**fetchTeamDarApplicationAnswers**](docs/DataAccessApplicationApi.md#fetchteamdarapplicationanswers) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/answers | DataAccessApplication@showAnswers
*DataAccessApplicationApi* | [**fetchTeamDarApplicationDownloadZip**](docs/DataAccessApplicationApi.md#fetchteamdarapplicationdownloadzip) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/download | DataAccessApplication@download
*DataAccessApplicationApi* | [**fetchTeamDarApplicationFile**](docs/DataAccessApplicationApi.md#fetchteamdarapplicationfile) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile
*DataAccessApplicationApi* | [**fetchTeamDarApplicationFiles**](docs/DataAccessApplicationApi.md#fetchteamdarapplicationfiles) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files | DataAccessApplication@showFiles
*DataAccessApplicationApi* | [**fetchTeamDarApplicationStatusHistory**](docs/DataAccessApplicationApi.md#fetchteamdarapplicationstatushistory) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/status | DataAccessApplication@status
*DataAccessApplicationApi* | [**updateTeamDarApplication**](docs/DataAccessApplicationApi.md#updateteamdarapplication) | **PATCH** /api/v1/teams/{teamId}/dar/applications/{id} | DataAccessApplication@update
*DataAccessApplicationReviewApi* | [**createTeamDarApplicationQuestionReview**](docs/DataAccessApplicationReviewApi.md#createteamdarapplicationquestionreview) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews | DataAccessApplicationReview@store
*DataAccessApplicationReviewApi* | [**createTeamDarApplicationReview**](docs/DataAccessApplicationReviewApi.md#createteamdarapplicationreview) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@storeGlobal
*DataAccessApplicationReviewApi* | [**deleteTeamDarApplicationQuestionReview**](docs/DataAccessApplicationReviewApi.md#deleteteamdarapplicationquestionreview) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@destroy
*DataAccessApplicationReviewApi* | [**deleteTeamDarApplicationReview**](docs/DataAccessApplicationReviewApi.md#deleteteamdarapplicationreview) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@destroyGlobal
*DataAccessApplicationReviewApi* | [**deleteTeamDarApplicationReviewFile**](docs/DataAccessApplicationReviewApi.md#deleteteamdarapplicationreviewfile) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/files/{fileId} | DataAccessApplicationReview@destroyFile
*DataAccessApplicationReviewApi* | [**fetchTeamDarApplicationReviewFile**](docs/DataAccessApplicationReviewApi.md#fetchteamdarapplicationreviewfile) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadFile
*DataAccessApplicationReviewApi* | [**fetchTeamDarApplicationReviews**](docs/DataAccessApplicationReviewApi.md#fetchteamdarapplicationreviews) | **GET** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@index
*DataAccessApplicationReviewApi* | [**updateTeamDarApplicationQuestionReview**](docs/DataAccessApplicationReviewApi.md#updateteamdarapplicationquestionreview) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@update
*DataAccessApplicationReviewApi* | [**updateTeamDarApplicationReview**](docs/DataAccessApplicationReviewApi.md#updateteamdarapplicationreview) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@updateGlobal
*DataAccessSectionApi* | [**createDarSection**](docs/DataAccessSectionApi.md#createdarsection) | **POST** /api/v1/dar/sections | DataAccessSection@store
*DataAccessSectionApi* | [**deleteDarSection**](docs/DataAccessSectionApi.md#deletedarsection) | **DELETE** /api/v1/dar/sections/{id} | DataAccessSection@destroy
*DataAccessSectionApi* | [**patchDarSection**](docs/DataAccessSectionApi.md#patchdarsection) | **PATCH** /api/v1/dar/sections/{id} | DataAccessSection@update
*DataAccessSectionApi* | [**updateDarSection**](docs/DataAccessSectionApi.md#updatedarsection) | **PUT** /api/v1/dar/sections/{id} | DataAccessSection@update
*DataAccessTemplateApi* | [**createDarTemplate**](docs/DataAccessTemplateApi.md#createdartemplate) | **POST** /api/v1/dar/templates | DataAccessTemplate@store
*DataAccessTemplateApi* | [**deleteDarTemplate**](docs/DataAccessTemplateApi.md#deletedartemplate) | **DELETE** /api/v1/dar/templates/{id} | DataAccessTemplate@destroy
*DataAccessTemplateApi* | [**fetchDarTemplate**](docs/DataAccessTemplateApi.md#fetchdartemplate) | **GET** /api/v1/dar/templates/{id} | DataAccessTemplate@show
*DataAccessTemplateApi* | [**fetchDarTemplates**](docs/DataAccessTemplateApi.md#fetchdartemplates) | **GET** /api/v1/dar/templates | DataAccessTemplate@index
*DataAccessTemplateApi* | [**patchDarTemplate**](docs/DataAccessTemplateApi.md#patchdartemplate) | **PATCH** /api/v1/dar/templates/{id} | DataAccessTemplate@update
*DataAccessTemplateApi* | [**updateDarTemplate**](docs/DataAccessTemplateApi.md#updatedartemplate) | **PUT** /api/v1/dar/templates/{id} | DataAccessTemplate@update
*DataAccessTemplatesApi* | [**darTemplateCountUniqueFields**](docs/DataAccessTemplatesApi.md#dartemplatecountuniquefields) | **GET** /api/v1/dar/templates/count/{field} | DataAccessTemplateController@count
*DataCustodianNetworksApi* | [**createDataCustodianNetwork**](docs/DataCustodianNetworksApi.md#createdatacustodiannetwork) | **POST** /api/v2/data_custodian_networks | DataCustodianNetworks@store
*DataCustodianNetworksApi* | [**deleteDataCustodianNetwork**](docs/DataCustodianNetworksApi.md#deletedatacustodiannetwork) | **DELETE** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@destroy
*DataCustodianNetworksApi* | [**editDataCustodianNetwork**](docs/DataCustodianNetworksApi.md#editdatacustodiannetwork) | **PATCH** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@edit
*DataCustodianNetworksApi* | [**fetchDataCustodianNetwork**](docs/DataCustodianNetworksApi.md#fetchdatacustodiannetwork) | **GET** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@show
*DataCustodianNetworksApi* | [**fetchDataCustodianNetworkCustodiansSummary**](docs/DataCustodianNetworksApi.md#fetchdatacustodiannetworkcustodianssummary) | **GET** /api/v2/data_custodian_networks/{id}/custodians_summary | DataCustodianNetworks@showCustodiansSummary
*DataCustodianNetworksApi* | [**fetchDataCustodianNetworkDatasetsSummary**](docs/DataCustodianNetworksApi.md#fetchdatacustodiannetworkdatasetssummary) | **GET** /api/v2/data_custodian_networks/{id}/datasets_summary | DataCustodianNetworks@showDatasetsSummary
*DataCustodianNetworksApi* | [**fetchDataCustodianNetworkEntitiesSummary**](docs/DataCustodianNetworksApi.md#fetchdatacustodiannetworkentitiessummary) | **GET** /api/v2/data_custodian_networks/{id}/entities_summary | DataCustodianNetworks@showSummary
*DataCustodianNetworksApi* | [**fetchDataCustodianNetworkInfo**](docs/DataCustodianNetworksApi.md#fetchdatacustodiannetworkinfo) | **GET** /api/v2/data_custodian_networks/{id}/info | DataCustodianNetworks@showInfoSummary
*DataCustodianNetworksApi* | [**fetchDataCustodianNetworks**](docs/DataCustodianNetworksApi.md#fetchdatacustodiannetworks) | **GET** /api/v2/data_custodian_networks | DataCustodianNetworks@index
*DataCustodianNetworksApi* | [**updateDataCustodianNetwork**](docs/DataCustodianNetworksApi.md#updatedatacustodiannetwork) | **PUT** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@update
*DataProviderCollApi* | [**createDataProviderColl**](docs/DataProviderCollApi.md#createdataprovidercoll) | **POST** /api/v1/data_provider_colls | DataProviderColl@store
*DataProviderCollApi* | [**deleteDataProviderColl**](docs/DataProviderCollApi.md#deletedataprovidercoll) | **DELETE** /api/v1/data_provider_colls/{id} | DataProviderColl@destroy
*DataProviderCollApi* | [**editDataProviderColl**](docs/DataProviderCollApi.md#editdataprovidercoll) | **PATCH** /api/v1/data_provider_colls/{id} | DataProviderColl@edit
*DataProviderCollApi* | [**fetchDataProviderColl**](docs/DataProviderCollApi.md#fetchdataprovidercoll) | **GET** /api/v1/data_provider_colls/{id} | DataProviderColl@show
*DataProviderCollApi* | [**fetchDataProviderCollSummary**](docs/DataProviderCollApi.md#fetchdataprovidercollsummary) | **GET** /api/v1/data_provider_colls/{id}/summary | DataProviderColl@showSummary
*DataProviderCollApi* | [**fetchDataProviderColls**](docs/DataProviderCollApi.md#fetchdataprovidercolls) | **GET** /api/v1/data_provider_colls | DataProviderColl@index
*DataProviderCollApi* | [**updateDataProviderColl**](docs/DataProviderCollApi.md#updatedataprovidercoll) | **PUT** /api/v1/data_provider_colls/{id} | DataProviderColl@update
*DataUseRegistersApi* | [**createDur**](docs/DataUseRegistersApi.md#createdur) | **POST** /api/v1/dur | DurController@store
*DataUseRegistersApi* | [**createDurByTeamV2**](docs/DataUseRegistersApi.md#createdurbyteamv2) | **POST** /api/v2/teams/{teamId}/dur | TeamDurController@store
*DataUseRegistersApi* | [**deleteDur**](docs/DataUseRegistersApi.md#deletedur) | **DELETE** /api/v1/dur/{id} | Delete a dur
*DataUseRegistersApi* | [**deleteDursV2ByTeamId**](docs/DataUseRegistersApi.md#deletedursv2byteamid) | **DELETE** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@destroy
*DataUseRegistersApi* | [**editDur**](docs/DataUseRegistersApi.md#editdur) | **PATCH** /api/v1/dur/{id} | Edit a dur
*DataUseRegistersApi* | [**editDursV2ByTeamId**](docs/DataUseRegistersApi.md#editdursv2byteamid) | **PATCH** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@edit
*DataUseRegistersApi* | [**exportDurTemplate**](docs/DataUseRegistersApi.md#exportdurtemplate) | **GET** /api/v1/dur/template | DurController@exportTemplate
*DataUseRegistersApi* | [**exportDurTemplateV2**](docs/DataUseRegistersApi.md#exportdurtemplatev2) | **GET** /api/v2/dur/template | DurController@exportTemplate
*DataUseRegistersApi* | [**exportDurV2**](docs/DataUseRegistersApi.md#exportdurv2) | **GET** /api/v2/dur/export | DurController@export
*DataUseRegistersApi* | [**fetchAllDur**](docs/DataUseRegistersApi.md#fetchalldur) | **GET** /api/v1/dur | DurController@index
*DataUseRegistersApi* | [**fetchAllDurV2**](docs/DataUseRegistersApi.md#fetchalldurv2) | **GET** /api/v2/dur | DurController@indexActive
*DataUseRegistersApi* | [**fetchDurById**](docs/DataUseRegistersApi.md#fetchdurbyid) | **GET** /api/v1/dur/{id} | DurController@show
*DataUseRegistersApi* | [**fetchDurByIdV2**](docs/DataUseRegistersApi.md#fetchdurbyidv2) | **GET** /api/v2/dur/{id} | DurController@showActive
*DataUseRegistersApi* | [**updateDur**](docs/DataUseRegistersApi.md#updatedur) | **PUT** /api/v1/dur/{id} | Update a dur by id
*DataUseRegistersApi* | [**updateDurV2ByTeamId**](docs/DataUseRegistersApi.md#updatedurv2byteamid) | **PUT** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@update
*DataUseRegistersApi* | [**uploadDur**](docs/DataUseRegistersApi.md#uploaddur) | **POST** /api/v1/dur/upload | DurController@upload
*DatasetsApi* | [**countUniqueFields**](docs/DatasetsApi.md#countuniquefields) | **GET** /api/v1/datasets/count/{field} | DatasetController@count
*DatasetsApi* | [**createDatasets**](docs/DatasetsApi.md#createdatasets) | **POST** /api/v1/datasets | DatasetController@store
*DatasetsApi* | [**createDatasetsIntegrations**](docs/DatasetsApi.md#createdatasetsintegrations) | **POST** /api/v1/integrations/datasets | IntegrationDatasetController@store
*DatasetsApi* | [**createDatasetsLinkageExtraction**](docs/DatasetsApi.md#createdatasetslinkageextraction) | **POST** /api/v1/datasets/admin_ctrl/trigger/linkage_extraction | Trigger Term Extraction for Datasets
*DatasetsApi* | [**createDatasetsTermExtraction**](docs/DatasetsApi.md#createdatasetstermextraction) | **POST** /api/v1/datasets/admin_ctrl/trigger/term_extraction | Trigger Term Extraction for Datasets
*DatasetsApi* | [**createDatasetsV2**](docs/DatasetsApi.md#createdatasetsv2) | **POST** /api/v2/datasets | DatasetController@store
*DatasetsApi* | [**createTeamDatasetsV2**](docs/DatasetsApi.md#createteamdatasetsv2) | **POST** /api/v2/teams/{teamId}/datasets | TeamDatasetController@store
*DatasetsApi* | [**deleteDatasets**](docs/DatasetsApi.md#deletedatasets) | **DELETE** /api/v1/datasets/{id} | DatasetController@destroy
*DatasetsApi* | [**deleteDatasetsIntegrations**](docs/DatasetsApi.md#deletedatasetsintegrations) | **DELETE** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@destroy
*DatasetsApi* | [**deleteDatasetsV2**](docs/DatasetsApi.md#deletedatasetsv2) | **DELETE** /api/v2/datasets/{id} | Delete a dataset
*DatasetsApi* | [**deleteTeamDatasetsV2**](docs/DatasetsApi.md#deleteteamdatasetsv2) | **DELETE** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@destroy
*DatasetsApi* | [**exportDatasetMetadata**](docs/DatasetsApi.md#exportdatasetmetadata) | **GET** /api/v1/datasets/export_metadata/{id} | DatasetController@exportMetadata
*DatasetsApi* | [**exportDatasets**](docs/DatasetsApi.md#exportdatasets) | **GET** /api/v1/datasets/export | DatasetController@export
*DatasetsApi* | [**exportDur**](docs/DatasetsApi.md#exportdur) | **GET** /api/v1/dur/export | DurController@export
*DatasetsApi* | [**exportMockDataset**](docs/DatasetsApi.md#exportmockdataset) | **GET** /api/v1/datasets/export/mock | DatasetController@exportMock
*DatasetsApi* | [**exportMockDatasetV2**](docs/DatasetsApi.md#exportmockdatasetv2) | **GET** /api/v2/datasets/export/mock | DatasetController@exportMock
*DatasetsApi* | [**fetchAllDatasets**](docs/DatasetsApi.md#fetchalldatasets) | **GET** /api/v1/datasets | DatasetController@index
*DatasetsApi* | [**fetchAllDatasetsIntegrations**](docs/DatasetsApi.md#fetchalldatasetsintegrations) | **GET** /api/v1/integrations/datasets | IntegrationDatasetController@index
*DatasetsApi* | [**fetchAllDatasetsV2**](docs/DatasetsApi.md#fetchalldatasetsv2) | **GET** /api/v2/datasets | DatasetController@index
*DatasetsApi* | [**fetchDatasets**](docs/DatasetsApi.md#fetchdatasets) | **GET** /api/v1/datasets/{id} | DatasetController@show
*DatasetsApi* | [**fetchDatasetsIntegrations**](docs/DatasetsApi.md#fetchdatasetsintegrations) | **GET** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@show
*DatasetsApi* | [**fetchDatasetsV2**](docs/DatasetsApi.md#fetchdatasetsv2) | **GET** /api/v2/datasets/{id} | DatasetController@showActive
*DatasetsApi* | [**patchDatasets**](docs/DatasetsApi.md#patchdatasets) | **PATCH** /api/v1/datasets/{id} | DatasetController@edit
*DatasetsApi* | [**patchDatasetsIntegrations**](docs/DatasetsApi.md#patchdatasetsintegrations) | **PATCH** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@edit
*DatasetsApi* | [**patchDatasetsV2**](docs/DatasetsApi.md#patchdatasetsv2) | **PATCH** /api/v2/datasets/{id} | DatasetController@edit
*DatasetsApi* | [**patchTeamDatasetsV2**](docs/DatasetsApi.md#patchteamdatasetsv2) | **PATCH** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@edit
*DatasetsApi* | [**updateDatasets**](docs/DatasetsApi.md#updatedatasets) | **PUT** /api/v1/datasets/{id} | DatasetController@update
*DatasetsApi* | [**updateDatasetsIntegrations**](docs/DatasetsApi.md#updatedatasetsintegrations) | **PUT** /api/v1/integrations/datasets/{id} | IntegrationDatasetController@update
*DatasetsApi* | [**updateDatasetsV2**](docs/DatasetsApi.md#updatedatasetsv2) | **PUT** /api/v2/datasets/{id} | DatasetController@update
*DatasetsApi* | [**updateTeamDatasetsV2**](docs/DatasetsApi.md#updateteamdatasetsv2) | **PUT** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@update
*DatasetsTestApi* | [**datasetsTest**](docs/DatasetsTestApi.md#datasetstest) | **POST** /api/v1/datasets/test | DatasetController@datasetTest
*FormHydrationApi* | [**getFormSchema**](docs/FormHydrationApi.md#getformschema) | **GET** /api/v1/form_hydration/schema | Retrieve form schema data
*FormHydrationApi* | [**onboardingFormHydration**](docs/FormHydrationApi.md#onboardingformhydration) | **GET** /api/v1/form_hydration | Retrieve form schema data
*IntegrationCollectionsApi* | [**createCollectionsIntegrations**](docs/IntegrationCollectionsApi.md#createcollectionsintegrations) | **POST** /api/v1/integrations/collections | IntegrationCollectionController@store
*IntegrationCollectionsApi* | [**deleteCollectionsIntegrations**](docs/IntegrationCollectionsApi.md#deletecollectionsintegrations) | **DELETE** /api/v1/integrations/collections/{id} | Delete a collection
*IntegrationCollectionsApi* | [**editCollectionsIntegrations**](docs/IntegrationCollectionsApi.md#editcollectionsintegrations) | **PATCH** /api/v1/integrations/collections/{id} | Edit a collection
*IntegrationCollectionsApi* | [**fetchAllCollectionsIntegrations**](docs/IntegrationCollectionsApi.md#fetchallcollectionsintegrations) | **GET** /api/v1/integrations/collections | IntegrationCollectionController@index
*IntegrationCollectionsApi* | [**fetchCollectionsIntegrations**](docs/IntegrationCollectionsApi.md#fetchcollectionsintegrations) | **GET** /api/v1/integrations/collections/{id} | IntegrationCollectionController@show
*IntegrationCollectionsApi* | [**updateCollectionsIntegrations**](docs/IntegrationCollectionsApi.md#updatecollectionsintegrations) | **PUT** /api/v1/integrations/collections/{id} | Update a collection
*IntegrationDataUseRegistersApi* | [**createDurIntegrations**](docs/IntegrationDataUseRegistersApi.md#createdurintegrations) | **POST** /api/v1/integrations/dur | IntegrationDurController@store
*IntegrationDataUseRegistersApi* | [**deleteDurIntegrations**](docs/IntegrationDataUseRegistersApi.md#deletedurintegrations) | **DELETE** /api/v1/integrations/dur/{id} | Delete a dur
*IntegrationDataUseRegistersApi* | [**editDurIntegrations**](docs/IntegrationDataUseRegistersApi.md#editdurintegrations) | **PATCH** /api/v1/integrations/dur/{id} | Edit a dur
*IntegrationDataUseRegistersApi* | [**fetchAllDurIntegrations**](docs/IntegrationDataUseRegistersApi.md#fetchalldurintegrations) | **GET** /api/v1/integrations/dur | IntegrationDurController@index
*IntegrationDataUseRegistersApi* | [**fetchDurByIdIntegrations**](docs/IntegrationDataUseRegistersApi.md#fetchdurbyidintegrations) | **GET** /api/v1/integrations/dur/{id} | IntegrationDurController@show
*IntegrationDataUseRegistersApi* | [**updateDurIntegrations**](docs/IntegrationDataUseRegistersApi.md#updatedurintegrations) | **PUT** /api/v1/integrations/dur/{id} | Update a dur by id
*IntegrationsDatasetsTestApi* | [**integrationsDatasetsTest**](docs/IntegrationsDatasetsTestApi.md#integrationsdatasetstest) | **POST** /api/v1/integrations/datasets/test | IntegrationDatasetController@datasetTest
*LicenseApi* | [**createLicenses**](docs/LicenseApi.md#createlicenses) | **POST** /api/v1/licenses | License@store
*LicenseApi* | [**deleteLicenses**](docs/LicenseApi.md#deletelicenses) | **DELETE** /api/v1/licenses/{id} | License@destroy
*LicenseApi* | [**editLicenses**](docs/LicenseApi.md#editlicenses) | **PATCH** /api/v1/licenses/{id} | License@edit
*LicenseApi* | [**fetchAllLicenses**](docs/LicenseApi.md#fetchalllicenses) | **GET** /api/v1/licenses | License@index
*LicenseApi* | [**fetchLicenses**](docs/LicenseApi.md#fetchlicenses) | **GET** /api/v1/licenses/{id} | License@show
*LicenseApi* | [**updateLicenses**](docs/LicenseApi.md#updatelicenses) | **PUT** /api/v1/licenses/{id} | License@update
*MetricsApi* | [**fetchKeyMetricsV2**](docs/MetricsApi.md#fetchkeymetricsv2) | **GET** /api/v2/metrics | KeyMetricController@index
*NotificationApi* | [**deleteNotifications**](docs/NotificationApi.md#deletenotifications) | **DELETE** /api/v1/notifications/{id} | Notification@destroy
*ProgrammingLanguageApi* | [**createProgrammingLanguages**](docs/ProgrammingLanguageApi.md#createprogramminglanguages) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store
*ProgrammingLanguageApi* | [**deleteProgrammingLanguages**](docs/ProgrammingLanguageApi.md#deleteprogramminglanguages) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy
*ProgrammingLanguageApi* | [**editProgrammingLanguages**](docs/ProgrammingLanguageApi.md#editprogramminglanguages) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update
*ProgrammingLanguageApi* | [**updateProgrammingLanguages**](docs/ProgrammingLanguageApi.md#updateprogramminglanguages) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update
*ProgrammingPackageApi* | [**createProgrammingPackages**](docs/ProgrammingPackageApi.md#createprogrammingpackages) | **POST** /api/v1/programming_packages | ProgrammingPackage@store
*ProgrammingPackageApi* | [**deleteProgrammingPackages**](docs/ProgrammingPackageApi.md#deleteprogrammingpackages) | **DELETE** /api/v1/programming_packages/{id} | ProgrammingPackage@destroy
*ProgrammingPackageApi* | [**editProgrammingPackages**](docs/ProgrammingPackageApi.md#editprogrammingpackages) | **PATCH** /api/v1/programming_packages/{id} | ProgrammingPackage@update
*ProgrammingPackageApi* | [**updateProgrammingPackages**](docs/ProgrammingPackageApi.md#updateprogrammingpackages) | **PUT** /api/v1/programming_packages/{id} | ProgrammingPackage@update
*ProjectGrantApi* | [**fetchAllProjectGrants**](docs/ProjectGrantApi.md#fetchallprojectgrants) | **GET** /api/v1/project_grants | ProjectGrantController@index
*ProjectGrantApi* | [**fetchProjectGrant**](docs/ProjectGrantApi.md#fetchprojectgrant) | **GET** /api/v1/project_grants/{id} | ProjectGrantController@show
*PublicationApi* | [**countUniqueFieldsPublications**](docs/PublicationApi.md#countuniquefieldspublications) | **GET** /api/v1/publication/count/{field} | PublicationController@count
*PublicationApi* | [**createPublications**](docs/PublicationApi.md#createpublications) | **POST** /api/v1/publications | PublicationController@store
*PublicationApi* | [**deletePublications**](docs/PublicationApi.md#deletepublications) | **DELETE** /api/v1/publications/{id} | PublicationController@destroy
*PublicationApi* | [**editPublications**](docs/PublicationApi.md#editpublications) | **PATCH** /api/v1/publications/{id} | PublicationController@edit
*PublicationApi* | [**fetchAllPublications**](docs/PublicationApi.md#fetchallpublications) | **GET** /api/v1/publications | PublicationController@index
*PublicationApi* | [**fetchAllPublicationsV2**](docs/PublicationApi.md#fetchallpublicationsv2) | **GET** /api/v2/publications | PublicationController@indexActive
*PublicationApi* | [**fetchPublications**](docs/PublicationApi.md#fetchpublications) | **GET** /api/v1/publications/{id} | PublicationController@show
*PublicationApi* | [**fetchPublicationsV2**](docs/PublicationApi.md#fetchpublicationsv2) | **GET** /api/v2/publications/{id} | PublicationController@showActive
*PublicationApi* | [**updatePublications**](docs/PublicationApi.md#updatepublications) | **PUT** /api/v1/publications/{id} | PublicationController@update
*QuestionBankApi* | [**createQuestionBankQuestion**](docs/QuestionBankApi.md#createquestionbankquestion) | **POST** /api/v1/questions | QuestionBank@store
*QuestionBankApi* | [**deleteQuestionBankQuestion**](docs/QuestionBankApi.md#deletequestionbankquestion) | **DELETE** /api/v1/questions/{id} | QuestionBank@destroy
*QuestionBankApi* | [**downloadQuestionBankQuestionFile**](docs/QuestionBankApi.md#downloadquestionbankquestionfile) | **GET** /api/v1/questions/{id}/files/{fileId} | QuestionBank@destroyFile
*QuestionBankApi* | [**editQuestionBankQuestion**](docs/QuestionBankApi.md#editquestionbankquestion) | **PATCH** /api/v1/questions/{id} | QuestionBank@update
*QuestionBankApi* | [**fetchArchivedQuestionBankQuestions**](docs/QuestionBankApi.md#fetcharchivedquestionbankquestions) | **GET** /api/v1/questions/archived | QuestionBank@indexArchived
*QuestionBankApi* | [**fetchCustomQuestionBankQuestions**](docs/QuestionBankApi.md#fetchcustomquestionbankquestions) | **GET** /api/v1/questions/custom | QuestionBank@indexCustom
*QuestionBankApi* | [**fetchQuestionBankQuestion**](docs/QuestionBankApi.md#fetchquestionbankquestion) | **GET** /api/v1/questions/{id} | QuestionBank@show
*QuestionBankApi* | [**fetchQuestionBankQuestionVersion**](docs/QuestionBankApi.md#fetchquestionbankquestionversion) | **GET** /api/v1/questions/version/{id} | QuestionBank@showVersion
*QuestionBankApi* | [**fetchQuestionBankQuestions**](docs/QuestionBankApi.md#fetchquestionbankquestions) | **GET** /api/v1/questions | QuestionBank@index
*QuestionBankApi* | [**fetchStandardQuestionBankQuestions**](docs/QuestionBankApi.md#fetchstandardquestionbankquestions) | **GET** /api/v1/questions/standard | QuestionBank@indexStandard
*QuestionBankApi* | [**fetchTeamQuestionBankQuestionsBySection**](docs/QuestionBankApi.md#fetchteamquestionbankquestionsbysection) | **GET** /api/v1/teams/{teamId}/questions/section/{sectionId} | TeamQuestionBank@indexBySection
*QuestionBankApi* | [**updateQuestionBankQuestion**](docs/QuestionBankApi.md#updatequestionbankquestion) | **PUT** /api/v1/questions/{id} | QuestionBank@update
*QuestionBankApi* | [**updateQuestionBankQuestionStatus**](docs/QuestionBankApi.md#updatequestionbankquestionstatus) | **PATCH** /api/v1/questions/{id}/{status} | QuestionBank@updateStatus
*ReviewsApi* | [**deleteReviews**](docs/ReviewsApi.md#deletereviews) | **DELETE** /api/v1/reviews/{id} | Delete a review
*ReviewsApi* | [**editReviews**](docs/ReviewsApi.md#editreviews) | **PATCH** /api/v1/reviews/{id} | Edit a review
*ReviewsApi* | [**updateReviews**](docs/ReviewsApi.md#updatereviews) | **PUT** /api/v1/reviews/{id} | Update a review
*SearchCollectionsApi* | [**searchCollections**](docs/SearchCollectionsApi.md#searchcollections) | **POST** /api/v1/search/collections | Search@collections
*SearchDataCustodianNetworksApi* | [**searchDataCustodianNetworks**](docs/SearchDataCustodianNetworksApi.md#searchdatacustodiannetworks) | **POST** /api/v1/search/data_custodian_networks | Search@data_custodian_networks
*SearchDataCustodiansApi* | [**searchDataCustodians**](docs/SearchDataCustodiansApi.md#searchdatacustodians) | **POST** /api/v1/search/data_custodians | Search@data_custodians
*SearchDataUsesApi* | [**searchDataUses**](docs/SearchDataUsesApi.md#searchdatauses) | **POST** /api/v1/search/dur | Search@data_uses
*SearchDatasetsApi* | [**searchDatasets**](docs/SearchDatasetsApi.md#searchdatasets) | **POST** /api/v1/search/datasets | Search@datasets
*SearchPublicationsApi* | [**searchPublications**](docs/SearchPublicationsApi.md#searchpublications) | **POST** /api/v1/search/publications | Search@publications
*SearchPublicationsApi* | [**searchPublicationsByDoi**](docs/SearchPublicationsApi.md#searchpublicationsbydoi) | **POST** /api/v1/search/doi | Search@publications
*SearchSimilarDatasetsApi* | [**searchSimilarDatasets**](docs/SearchSimilarDatasetsApi.md#searchsimilardatasets) | **POST** /api/v1/search/similar/datasets | Search@similarDatasets
*SearchToolsApi* | [**searchTools**](docs/SearchToolsApi.md#searchtools) | **POST** /api/v1/search/tools | Search@tools
*TeamDataAccessApplicationApi* | [**countTeamDarApplications**](docs/TeamDataAccessApplicationApi.md#countteamdarapplications) | **GET** /api/v1/teams/{teamId}/dar/applications/count | TeamDataAccessApplicationController@allCounts
*TeamDataAccessApplicationApi* | [**countUniqueFieldsDarApplications**](docs/TeamDataAccessApplicationApi.md#countuniquefieldsdarapplications) | **GET** /api/v1/teams/{teamId}/dar/applications/count/{field} | TeamDataAccessApplicationController@count
*TeamDataAccessApplicationApi* | [**fetchTeamDarApplication**](docs/TeamDataAccessApplicationApi.md#fetchteamdarapplication) | **GET** /api/v1/teams/{teamId}/dar/applications/{id} | TeamDataAccessApplicationController@show
*TeamDataAccessApplicationApi* | [**fetchTeamDarApplications**](docs/TeamDataAccessApplicationApi.md#fetchteamdarapplications) | **GET** /api/v1/teams/{teamId}/dar/applications | TeamDataAccessApplicationController@index
*TeamDataAccessTemplateApi* | [**deleteTeamDarTemplateFile**](docs/TeamDataAccessTemplateApi.md#deleteteamdartemplatefile) | **DELETE** /api/v1/teams/{teamId}/dar/templates/{id}/files/{fileId} | TeamDataAccessTemplateController@destroyFile
*TeamDataAccessTemplateApi* | [**fetchTeamDarTemplates**](docs/TeamDataAccessTemplateApi.md#fetchteamdartemplates) | **GET** /api/v1/teams/{teamId}/dar/templates | TeamDataAccessTemplateController@index
*TeamDataAccessTemplateApi* | [**teamDarTemplateCountUniqueFields**](docs/TeamDataAccessTemplateApi.md#teamdartemplatecountuniquefields) | **GET** /api/v1/teams/{teamId}/dar/templates/count/{field} | TeamDataAccessTemplateController@count
*TeamFederationsApi* | [**createFederationTeam**](docs/TeamFederationsApi.md#createfederationteam) | **POST** /api/v1/teams/{teamId}/federations | FederationController@store
*TeamFederationsApi* | [**deleteFederation**](docs/TeamFederationsApi.md#deletefederation) | **DELETE** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@destroy
*TeamFederationsApi* | [**editFederationTeam**](docs/TeamFederationsApi.md#editfederationteam) | **PATCH** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@edit
*TeamFederationsApi* | [**getFederationByFederationIdAndTeamId**](docs/TeamFederationsApi.md#getfederationbyfederationidandteamid) | **GET** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@show
*TeamFederationsApi* | [**getFederationHistory**](docs/TeamFederationsApi.md#getfederationhistory) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/history | FederationController@history
*TeamFederationsApi* | [**getFederationTeamId**](docs/TeamFederationsApi.md#getfederationteamid) | **GET** /api/v1/teams/{teamId}/federations | FederationController@index
*TeamFederationsApi* | [**runFederation**](docs/TeamFederationsApi.md#runfederation) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/run | FederationController@runNow
*TeamFederationsApi* | [**testFederation**](docs/TeamFederationsApi.md#testfederation) | **POST** /api/v1/teams/{teamId}/federations/test | FederationController@testFederation
*TeamFederationsApi* | [**updateFederationTeam**](docs/TeamFederationsApi.md#updatefederationteam) | **PUT** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@update
*ToolsApi* | [**countUniqueFieldsTools**](docs/ToolsApi.md#countuniquefieldstools) | **GET** /api/v1/tools/count/{field} | ToolController@count
*ToolsApi* | [**createTools**](docs/ToolsApi.md#createtools) | **POST** /api/v1/tools | ToolController@store
*ToolsApi* | [**createToolsByTeamV2**](docs/ToolsApi.md#createtoolsbyteamv2) | **POST** /api/v2/teams/{teamId}/tools | ToolController@store
*ToolsApi* | [**createToolsIntegrations**](docs/ToolsApi.md#createtoolsintegrations) | **POST** /api/v1/integrations/tools | IntegrationToolController@store
*ToolsApi* | [**deleteTools**](docs/ToolsApi.md#deletetools) | **DELETE** /api/v1/tools/{id} | ToolController@destroy
*ToolsApi* | [**deleteToolsByTeamidV2**](docs/ToolsApi.md#deletetoolsbyteamidv2) | **DELETE** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@destroy
*ToolsApi* | [**deleteToolsIntegrations**](docs/ToolsApi.md#deletetoolsintegrations) | **DELETE** /api/v1/integrations/tools/{id} | IntegrationToolController@destroy
*ToolsApi* | [**editTools**](docs/ToolsApi.md#edittools) | **PATCH** /api/v1/tools/{id} | ToolController@edit
*ToolsApi* | [**editToolsByTeamidV2**](docs/ToolsApi.md#edittoolsbyteamidv2) | **PATCH** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@edit
*ToolsApi* | [**editToolsIntegrations**](docs/ToolsApi.md#edittoolsintegrations) | **PATCH** /api/v1/integrations/tools/{id} | IntegrationToolController@edit
*ToolsApi* | [**fetchAllTools**](docs/ToolsApi.md#fetchalltools) | **GET** /api/v1/tools | Fetch all tools
*ToolsApi* | [**fetchAllToolsIntegrations**](docs/ToolsApi.md#fetchalltoolsintegrations) | **GET** /api/v1/integrations/tools | IntegrationToolController@index
*ToolsApi* | [**fetchAllToolsV2**](docs/ToolsApi.md#fetchalltoolsv2) | **GET** /api/v2/tools | ToolController@indexActive
*ToolsApi* | [**fetchTools**](docs/ToolsApi.md#fetchtools) | **GET** /api/v1/tools/{id} | ToolController@show
*ToolsApi* | [**fetchToolsIntegrations**](docs/ToolsApi.md#fetchtoolsintegrations) | **GET** /api/v1/integrations/tools/{id} | IntegrationToolController@show
*ToolsApi* | [**fetchToolsV2**](docs/ToolsApi.md#fetchtoolsv2) | **GET** /api/v2/tools/{id} | ToolController@showActive
*ToolsApi* | [**updateTools**](docs/ToolsApi.md#updatetools) | **PUT** /api/v1/tools/{id} | ToolController@update
*ToolsApi* | [**updateToolsByTeamidV2**](docs/ToolsApi.md#updatetoolsbyteamidv2) | **PUT** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@update
*ToolsApi* | [**updateToolsIntegrations**](docs/ToolsApi.md#updatetoolsintegrations) | **PUT** /api/v1/integrations/tools/{id} | IntegrationToolController@update
*TypeCategoryApi* | [**createTypeCategories**](docs/TypeCategoryApi.md#createtypecategories) | **POST** /api/v1/type_categories | TypeCategory@store
*TypeCategoryApi* | [**deleteTypeCategories**](docs/TypeCategoryApi.md#deletetypecategories) | **DELETE** /api/v1/type_categories/{id} | TypeCategory@destroy
*TypeCategoryApi* | [**editTypeCategories**](docs/TypeCategoryApi.md#edittypecategories) | **PATCH** /api/v1/type_categories/{id} | TypeCategory@update
*TypeCategoryApi* | [**updateTypeCategories**](docs/TypeCategoryApi.md#updatetypecategories) | **PUT** /api/v1/type_categories/{id} | TypeCategory@update
*UserRolesApi* | [**createUserHasRoles**](docs/UserRolesApi.md#createuserhasroles) | **POST** /api/v1/users/{userId}/roles | UserRoleController@store
*UserRolesApi* | [**deleteUserHasRoles**](docs/UserRolesApi.md#deleteuserhasroles) | **DELETE** /api/v1/users/{userId}/roles | UserRoleController@destroy
*UserRolesApi* | [**updateUserHasRoles**](docs/UserRolesApi.md#updateuserhasroles) | **PATCH** /api/v1/users/{userId}/roles | UserRoleController@edit
*UsersApi* | [**createUsers**](docs/UsersApi.md#createusers) | **POST** /api/v1/users | UserController@store
*UsersApi* | [**deleteUsers**](docs/UsersApi.md#deleteusers) | **DELETE** /api/v1/users/{id} | UserController@destroy
*UsersApi* | [**editUsers**](docs/UsersApi.md#editusers) | **PATCH** /api/v1/users/{id} | UserController@edit
*UsersApi* | [**verifySecondaryEmail**](docs/UsersApi.md#verifysecondaryemail) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user\&#39;s secondary email using a UUID
*WidgetsApi* | [**createWidget**](docs/WidgetsApi.md#createwidget) | **POST** /api/v1/teams/{teamId}/widgets | Create a new widget
*WidgetsApi* | [**deleteWidget**](docs/WidgetsApi.md#deletewidget) | **DELETE** /api/v1/teams/{teamId}/widgets/{id} | Delete a widget
*WidgetsApi* | [**fetchAllWidgets**](docs/WidgetsApi.md#fetchallwidgets) | **GET** /api/v1/teams/{teamId}/widgets | WidgetController@index
*WidgetsApi* | [**fetchWidget**](docs/WidgetsApi.md#fetchwidget) | **GET** /api/v1/teams/{teamId}/widgets/{id} | WidgetController@retrieve
*WidgetsApi* | [**fetchWidgetDataSources**](docs/WidgetsApi.md#fetchwidgetdatasources) | **GET** /api/v1/teams/{teamId}/widgets/data | WidgetController@getWidgetData
*WidgetsApi* | [**retrieveWidgetData**](docs/WidgetsApi.md#retrievewidgetdata) | **GET** /api/v1/teams/{teamId}/widgets/{id}/data | Retrieve data related to a widget
*WidgetsApi* | [**trackWidgetEvent**](docs/WidgetsApi.md#trackwidgetevent) | **POST** /api/v1/teams/{teamId}/widgets/{id}/track | Record a widget analytics event
*WidgetsApi* | [**updateWidget**](docs/WidgetsApi.md#updatewidget) | **PATCH** /api/v1/teams/{teamId}/widgets/{id} | Update an existing widget
*WidgetsApi* | [**widgetAnalytics**](docs/WidgetsApi.md#widgetanalytics) | **GET** /api/v1/teams/{teamId}/widgets/analytics | Get widget analytics for a team


### Documentation For Models

 - [Alias](docs/Alias.md)
 - [Authentication200Response](docs/Authentication200Response.md)
 - [AuthenticationRequest](docs/AuthenticationRequest.md)
 - [Category](docs/Category.md)
 - [Collection](docs/Collection.md)
 - [CountUniqueFieldsCollections200Response](docs/CountUniqueFieldsCollections200Response.md)
 - [CreateAdminSearchReindexRequest](docs/CreateAdminSearchReindexRequest.md)
 - [CreateApplications200Response](docs/CreateApplications200Response.md)
 - [CreateApplications200ResponseDataInner](docs/CreateApplications200ResponseDataInner.md)
 - [CreateApplications500Response](docs/CreateApplications500Response.md)
 - [CreateApplicationsRequest](docs/CreateApplicationsRequest.md)
 - [CreateCollectionsIntegrationsRequest](docs/CreateCollectionsIntegrationsRequest.md)
 - [CreateCollectionsIntegrationsRequestDatasetsInner](docs/CreateCollectionsIntegrationsRequestDatasetsInner.md)
 - [CreateCollectionsRequest](docs/CreateCollectionsRequest.md)
 - [CreateCsat422Response](docs/CreateCsat422Response.md)
 - [CreateCsatRequest](docs/CreateCsatRequest.md)
 - [CreateDarIntegration201Response](docs/CreateDarIntegration201Response.md)
 - [CreateDarSectionRequest](docs/CreateDarSectionRequest.md)
 - [CreateDarTemplateRequest](docs/CreateDarTemplateRequest.md)
 - [CreateDarTemplateRequestQuestionsInner](docs/CreateDarTemplateRequestQuestionsInner.md)
 - [CreateDataProviderCollRequest](docs/CreateDataProviderCollRequest.md)
 - [CreateDatasetsLinkageExtraction200Response](docs/CreateDatasetsLinkageExtraction200Response.md)
 - [CreateDatasetsLinkageExtractionRequest](docs/CreateDatasetsLinkageExtractionRequest.md)
 - [CreateDatasetsRequest](docs/CreateDatasetsRequest.md)
 - [CreateDatasetsTermExtraction200Response](docs/CreateDatasetsTermExtraction200Response.md)
 - [CreateDatasetsTermExtraction500Response](docs/CreateDatasetsTermExtraction500Response.md)
 - [CreateDatasetsTermExtractionRequest](docs/CreateDatasetsTermExtractionRequest.md)
 - [CreateDatasetsV2Request](docs/CreateDatasetsV2Request.md)
 - [CreateDurIntegrationsRequest](docs/CreateDurIntegrationsRequest.md)
 - [CreateDurRequest](docs/CreateDurRequest.md)
 - [CreateDurRequestDatasetsInner](docs/CreateDurRequestDatasetsInner.md)
 - [CreateDurRequestPublicationsInner](docs/CreateDurRequestPublicationsInner.md)
 - [CreateDurRequestTeamInner](docs/CreateDurRequestTeamInner.md)
 - [CreateDurRequestUsersInner](docs/CreateDurRequestUsersInner.md)
 - [CreateFederationTeamRequest](docs/CreateFederationTeamRequest.md)
 - [CreateLicensesRequest](docs/CreateLicensesRequest.md)
 - [CreateProgrammingLanguagesRequest](docs/CreateProgrammingLanguagesRequest.md)
 - [CreatePublicationsRequest](docs/CreatePublicationsRequest.md)
 - [CreatePublicationsRequestDatasetsInner](docs/CreatePublicationsRequestDatasetsInner.md)
 - [CreatePublicationsRequestToolsInner](docs/CreatePublicationsRequestToolsInner.md)
 - [CreateQuestionBankQuestionRequest](docs/CreateQuestionBankQuestionRequest.md)
 - [CreateQuestionBankQuestionRequestOptionsInner](docs/CreateQuestionBankQuestionRequestOptionsInner.md)
 - [CreateQuestionBankQuestionRequestOptionsInnerChildrenInner](docs/CreateQuestionBankQuestionRequestOptionsInnerChildrenInner.md)
 - [CreateQuestionBankQuestionRequestOptionsInnerChildrenInnerOptionsInner](docs/CreateQuestionBankQuestionRequestOptionsInnerChildrenInnerOptionsInner.md)
 - [CreateTeamDarApplicationReviewRequest](docs/CreateTeamDarApplicationReviewRequest.md)
 - [CreateTeamDatasetsV2Request](docs/CreateTeamDatasetsV2Request.md)
 - [CreateToolsIntegrations400Response](docs/CreateToolsIntegrations400Response.md)
 - [CreateToolsIntegrationsRequest](docs/CreateToolsIntegrationsRequest.md)
 - [CreateToolsIntegrationsRequestDatasetInner](docs/CreateToolsIntegrationsRequestDatasetInner.md)
 - [CreateToolsIntegrationsRequestPublicationsInner](docs/CreateToolsIntegrationsRequestPublicationsInner.md)
 - [CreateToolsRequest](docs/CreateToolsRequest.md)
 - [CreateToolsRequestCollectionsInner](docs/CreateToolsRequestCollectionsInner.md)
 - [CreateTypeCategoriesRequest](docs/CreateTypeCategoriesRequest.md)
 - [CreateUserHasRolesRequest](docs/CreateUserHasRolesRequest.md)
 - [CreateUsersRequest](docs/CreateUsersRequest.md)
 - [CreateWidget201Response](docs/CreateWidget201Response.md)
 - [CreateWidget400Response](docs/CreateWidget400Response.md)
 - [CreateWidgetRequest](docs/CreateWidgetRequest.md)
 - [DataAccessApplication](docs/DataAccessApplication.md)
 - [DataAccessApplicationReview](docs/DataAccessApplicationReview.md)
 - [DataCustodianNetwork](docs/DataCustodianNetwork.md)
 - [Dataset](docs/Dataset.md)
 - [DatasetVersion](docs/DatasetVersion.md)
 - [DatasetsTestRequest](docs/DatasetsTestRequest.md)
 - [DeleteApplications200Response](docs/DeleteApplications200Response.md)
 - [DeleteFederation200Response](docs/DeleteFederation200Response.md)
 - [DeleteFederation404Response](docs/DeleteFederation404Response.md)
 - [Dur](docs/Dur.md)
 - [EditApplicationsRequest](docs/EditApplicationsRequest.md)
 - [EditCollectionsV2Request](docs/EditCollectionsV2Request.md)
 - [EditCsat200Response](docs/EditCsat200Response.md)
 - [EditCsatRequest](docs/EditCsatRequest.md)
 - [EditDarIntegrationRequest](docs/EditDarIntegrationRequest.md)
 - [EditDataProviderCollRequest](docs/EditDataProviderCollRequest.md)
 - [EditProgrammingLanguagesRequest](docs/EditProgrammingLanguagesRequest.md)
 - [EditQuestionBankQuestionRequest](docs/EditQuestionBankQuestionRequest.md)
 - [EditUsers200Response](docs/EditUsers200Response.md)
 - [EditUsersRequest](docs/EditUsersRequest.md)
 - [ExportDatasetMetadata400Response](docs/ExportDatasetMetadata400Response.md)
 - [ExportMockDataset404Response](docs/ExportMockDataset404Response.md)
 - [FetchAllApplications200Response](docs/FetchAllApplications200Response.md)
 - [FetchAllApplications200ResponseDataInner](docs/FetchAllApplications200ResponseDataInner.md)
 - [FetchAllCollections200Response](docs/FetchAllCollections200Response.md)
 - [FetchAllDarIntegrations200Response](docs/FetchAllDarIntegrations200Response.md)
 - [FetchAllDarIntegrations200ResponseDataInner](docs/FetchAllDarIntegrations200ResponseDataInner.md)
 - [FetchAllDarIntegrations401Response](docs/FetchAllDarIntegrations401Response.md)
 - [FetchAllDatasets200Response](docs/FetchAllDatasets200Response.md)
 - [FetchAllDur200Response](docs/FetchAllDur200Response.md)
 - [FetchAllDurIntegrations200Response](docs/FetchAllDurIntegrations200Response.md)
 - [FetchAllDurIntegrations200ResponseDataInner](docs/FetchAllDurIntegrations200ResponseDataInner.md)
 - [FetchAllDurV2200Response](docs/FetchAllDurV2200Response.md)
 - [FetchAllLicenses200Response](docs/FetchAllLicenses200Response.md)
 - [FetchAllProjectGrants200Response](docs/FetchAllProjectGrants200Response.md)
 - [FetchAllPublications200Response](docs/FetchAllPublications200Response.md)
 - [FetchAllSitemap200Response](docs/FetchAllSitemap200Response.md)
 - [FetchAllSitemap200ResponseDataInner](docs/FetchAllSitemap200ResponseDataInner.md)
 - [FetchAllTools200Response](docs/FetchAllTools200Response.md)
 - [FetchAllTools500Response](docs/FetchAllTools500Response.md)
 - [FetchAllToolsIntegrations200Response](docs/FetchAllToolsIntegrations200Response.md)
 - [FetchAllWidgets200Response](docs/FetchAllWidgets200Response.md)
 - [FetchApplications200Response](docs/FetchApplications200Response.md)
 - [FetchApplications200ResponseDataInner](docs/FetchApplications200ResponseDataInner.md)
 - [FetchCollections200Response](docs/FetchCollections200Response.md)
 - [FetchCustomQuestionBankQuestions200Response](docs/FetchCustomQuestionBankQuestions200Response.md)
 - [FetchDarTemplate200Response](docs/FetchDarTemplate200Response.md)
 - [FetchDarTemplates200Response](docs/FetchDarTemplates200Response.md)
 - [FetchDarTemplates200ResponseDataInner](docs/FetchDarTemplates200ResponseDataInner.md)
 - [FetchDataCustodianNetwork200Response](docs/FetchDataCustodianNetwork200Response.md)
 - [FetchDataCustodianNetworkCustodiansSummary200Response](docs/FetchDataCustodianNetworkCustodiansSummary200Response.md)
 - [FetchDataCustodianNetworkCustodiansSummary200ResponseData](docs/FetchDataCustodianNetworkCustodiansSummary200ResponseData.md)
 - [FetchDataCustodianNetworkDatasetsSummary200Response](docs/FetchDataCustodianNetworkDatasetsSummary200Response.md)
 - [FetchDataCustodianNetworkDatasetsSummary200ResponseData](docs/FetchDataCustodianNetworkDatasetsSummary200ResponseData.md)
 - [FetchDataCustodianNetworkEntitiesSummary200Response](docs/FetchDataCustodianNetworkEntitiesSummary200Response.md)
 - [FetchDataCustodianNetworkEntitiesSummary200ResponseData](docs/FetchDataCustodianNetworkEntitiesSummary200ResponseData.md)
 - [FetchDataCustodianNetworkInfo200Response](docs/FetchDataCustodianNetworkInfo200Response.md)
 - [FetchDataCustodianNetworkInfo200ResponseData](docs/FetchDataCustodianNetworkInfo200ResponseData.md)
 - [FetchDataCustodianNetworks200Response](docs/FetchDataCustodianNetworks200Response.md)
 - [FetchDataProviderColl200Response](docs/FetchDataProviderColl200Response.md)
 - [FetchDataProviderCollSummary200Response](docs/FetchDataProviderCollSummary200Response.md)
 - [FetchDataProviderCollSummary200ResponseData](docs/FetchDataProviderCollSummary200ResponseData.md)
 - [FetchDataProviderColls200Response](docs/FetchDataProviderColls200Response.md)
 - [FetchDataProviderColls200ResponseDataInner](docs/FetchDataProviderColls200ResponseDataInner.md)
 - [FetchDatasets200Response](docs/FetchDatasets200Response.md)
 - [FetchDurById200Response](docs/FetchDurById200Response.md)
 - [FetchDurByIdIntegrations200Response](docs/FetchDurByIdIntegrations200Response.md)
 - [FetchDurByIdIntegrations200ResponseDataInner](docs/FetchDurByIdIntegrations200ResponseDataInner.md)
 - [FetchKeyMetricsV2200Response](docs/FetchKeyMetricsV2200Response.md)
 - [FetchLicenses200Response](docs/FetchLicenses200Response.md)
 - [FetchPublications200Response](docs/FetchPublications200Response.md)
 - [FetchQuestionBankQuestion200Response](docs/FetchQuestionBankQuestion200Response.md)
 - [FetchQuestionBankQuestion200ResponseData](docs/FetchQuestionBankQuestion200ResponseData.md)
 - [FetchQuestionBankQuestionVersion200Response](docs/FetchQuestionBankQuestionVersion200Response.md)
 - [FetchQuestionBankQuestionVersion200ResponseData](docs/FetchQuestionBankQuestionVersion200ResponseData.md)
 - [FetchQuestionBankQuestions200Response](docs/FetchQuestionBankQuestions200Response.md)
 - [FetchStandardQuestionBankQuestions200Response](docs/FetchStandardQuestionBankQuestions200Response.md)
 - [FetchTeamDarApplication200Response](docs/FetchTeamDarApplication200Response.md)
 - [FetchTeamDarApplicationAnswers200Response](docs/FetchTeamDarApplicationAnswers200Response.md)
 - [FetchTeamDarApplicationAnswers200ResponseData](docs/FetchTeamDarApplicationAnswers200ResponseData.md)
 - [FetchTeamDarApplicationFiles200Response](docs/FetchTeamDarApplicationFiles200Response.md)
 - [FetchTeamDarApplicationFiles200ResponseData](docs/FetchTeamDarApplicationFiles200ResponseData.md)
 - [FetchTeamDarApplicationReviews200Response](docs/FetchTeamDarApplicationReviews200Response.md)
 - [FetchTeamDarApplicationStatusHistory200Response](docs/FetchTeamDarApplicationStatusHistory200Response.md)
 - [FetchTeamDarApplicationStatusHistory200ResponseData](docs/FetchTeamDarApplicationStatusHistory200ResponseData.md)
 - [FetchTeamDarApplications200Response](docs/FetchTeamDarApplications200Response.md)
 - [FetchTeamQuestionBankQuestionsBySection200Response](docs/FetchTeamQuestionBankQuestionsBySection200Response.md)
 - [FetchTeamQuestionBankQuestionsBySection200ResponseDataInner](docs/FetchTeamQuestionBankQuestionsBySection200ResponseDataInner.md)
 - [FetchToolsIntegrations200Response](docs/FetchToolsIntegrations200Response.md)
 - [FetchWidget200Response](docs/FetchWidget200Response.md)
 - [FetchWidgetDataSources200Response](docs/FetchWidgetDataSources200Response.md)
 - [FetchWidgetDataSources400Response](docs/FetchWidgetDataSources400Response.md)
 - [GetCancerTypeFilter200Response](docs/GetCancerTypeFilter200Response.md)
 - [GetCancerTypeFilter404Response](docs/GetCancerTypeFilter404Response.md)
 - [GetCancerTypeFilters200Response](docs/GetCancerTypeFilters200Response.md)
 - [GetCancerTypeFilters200ResponseDataInner](docs/GetCancerTypeFilters200ResponseDataInner.md)
 - [GetFederationByFederationIdAndTeamId200Response](docs/GetFederationByFederationIdAndTeamId200Response.md)
 - [GetFederationByFederationIdAndTeamId200ResponseData](docs/GetFederationByFederationIdAndTeamId200ResponseData.md)
 - [GetFederationHistory200Response](docs/GetFederationHistory200Response.md)
 - [GetFederationHistory200ResponseDataInner](docs/GetFederationHistory200ResponseDataInner.md)
 - [GetFederationHistory200ResponseDataInnerFailedDatasetsInner](docs/GetFederationHistory200ResponseDataInnerFailedDatasetsInner.md)
 - [GetFederationTeamId200Response](docs/GetFederationTeamId200Response.md)
 - [GetFederationTeamId200ResponseDataInner](docs/GetFederationTeamId200ResponseDataInner.md)
 - [Keyword](docs/Keyword.md)
 - [License](docs/License.md)
 - [LoginRequest](docs/LoginRequest.md)
 - [Notification](docs/Notification.md)
 - [PatchDarSectionRequest](docs/PatchDarSectionRequest.md)
 - [PatchDarTemplate200Response](docs/PatchDarTemplate200Response.md)
 - [PatchDarTemplate200ResponseData](docs/PatchDarTemplate200ResponseData.md)
 - [PatchDarTemplateRequest](docs/PatchDarTemplateRequest.md)
 - [PatchDatasetsV2Request](docs/PatchDatasetsV2Request.md)
 - [ProgrammingLanguage](docs/ProgrammingLanguage.md)
 - [ProgrammingPackage](docs/ProgrammingPackage.md)
 - [Publication](docs/Publication.md)
 - [QuestionBank](docs/QuestionBank.md)
 - [Register200Response](docs/Register200Response.md)
 - [Register200ResponseUser](docs/Register200ResponseUser.md)
 - [RegisterRequest](docs/RegisterRequest.md)
 - [RetrieveWidgetData200Response](docs/RetrieveWidgetData200Response.md)
 - [RetrieveWidgetData403Response](docs/RetrieveWidgetData403Response.md)
 - [SavedSearch](docs/SavedSearch.md)
 - [SearchCollections200Response](docs/SearchCollections200Response.md)
 - [SearchCollections200ResponseDataInner](docs/SearchCollections200ResponseDataInner.md)
 - [SearchCollections200ResponseDataInnerSourceInner](docs/SearchCollections200ResponseDataInnerSourceInner.md)
 - [SearchCollectionsRequest](docs/SearchCollectionsRequest.md)
 - [SearchDataCustodianNetworks200Response](docs/SearchDataCustodianNetworks200Response.md)
 - [SearchDataCustodianNetworks200ResponseDataInner](docs/SearchDataCustodianNetworks200ResponseDataInner.md)
 - [SearchDataCustodianNetworks200ResponseDataInnerSourceInner](docs/SearchDataCustodianNetworks200ResponseDataInnerSourceInner.md)
 - [SearchDataCustodianNetworksRequest](docs/SearchDataCustodianNetworksRequest.md)
 - [SearchDataCustodians200Response](docs/SearchDataCustodians200Response.md)
 - [SearchDataCustodians200ResponseDataInner](docs/SearchDataCustodians200ResponseDataInner.md)
 - [SearchDataCustodians200ResponseDataInnerSourceInner](docs/SearchDataCustodians200ResponseDataInnerSourceInner.md)
 - [SearchDataCustodiansRequest](docs/SearchDataCustodiansRequest.md)
 - [SearchDataUses200Response](docs/SearchDataUses200Response.md)
 - [SearchDataUses200ResponseDataInner](docs/SearchDataUses200ResponseDataInner.md)
 - [SearchDataUses200ResponseDataInnerHighlightInner](docs/SearchDataUses200ResponseDataInnerHighlightInner.md)
 - [SearchDataUses200ResponseDataInnerSourceInner](docs/SearchDataUses200ResponseDataInnerSourceInner.md)
 - [SearchDataUsesRequest](docs/SearchDataUsesRequest.md)
 - [SearchDatasets200Response](docs/SearchDatasets200Response.md)
 - [SearchDatasets200ResponseDataInner](docs/SearchDatasets200ResponseDataInner.md)
 - [SearchDatasets200ResponseDataInnerHighlightInner](docs/SearchDatasets200ResponseDataInnerHighlightInner.md)
 - [SearchDatasets200ResponseDataInnerSourceInner](docs/SearchDatasets200ResponseDataInnerSourceInner.md)
 - [SearchDatasetsRequest](docs/SearchDatasetsRequest.md)
 - [SearchPublications200Response](docs/SearchPublications200Response.md)
 - [SearchPublications200ResponseDataInner](docs/SearchPublications200ResponseDataInner.md)
 - [SearchPublications200ResponseDataInnerHighlightInner](docs/SearchPublications200ResponseDataInnerHighlightInner.md)
 - [SearchPublications200ResponseDataInnerSourceInner](docs/SearchPublications200ResponseDataInnerSourceInner.md)
 - [SearchPublicationsByDoi200Response](docs/SearchPublicationsByDoi200Response.md)
 - [SearchPublicationsByDoiRequest](docs/SearchPublicationsByDoiRequest.md)
 - [SearchPublicationsRequest](docs/SearchPublicationsRequest.md)
 - [SearchSimilarDatasets200Response](docs/SearchSimilarDatasets200Response.md)
 - [SearchSimilarDatasets200ResponseDataInner](docs/SearchSimilarDatasets200ResponseDataInner.md)
 - [SearchSimilarDatasetsRequest](docs/SearchSimilarDatasetsRequest.md)
 - [SearchTools200Response](docs/SearchTools200Response.md)
 - [SearchTools200ResponseDataInner](docs/SearchTools200ResponseDataInner.md)
 - [SearchTools200ResponseDataInnerHighlightInner](docs/SearchTools200ResponseDataInnerHighlightInner.md)
 - [SearchTools200ResponseDataInnerSourceInner](docs/SearchTools200ResponseDataInnerSourceInner.md)
 - [SearchToolsRequest](docs/SearchToolsRequest.md)
 - [Team](docs/Team.md)
 - [TestFederation200Response](docs/TestFederation200Response.md)
 - [Tool](docs/Tool.md)
 - [TrackWidgetEventRequest](docs/TrackWidgetEventRequest.md)
 - [TypeCategory](docs/TypeCategory.md)
 - [UpdateAdminSearchFeatureRequest](docs/UpdateAdminSearchFeatureRequest.md)
 - [UpdateApplications200Response](docs/UpdateApplications200Response.md)
 - [UpdateApplications200ResponseData](docs/UpdateApplications200ResponseData.md)
 - [UpdateApplications404Response](docs/UpdateApplications404Response.md)
 - [UpdateApplicationsRequest](docs/UpdateApplicationsRequest.md)
 - [UpdateCollectionsV2Request](docs/UpdateCollectionsV2Request.md)
 - [UpdateDarIntegration200Response](docs/UpdateDarIntegration200Response.md)
 - [UpdateDarIntegrationRequest](docs/UpdateDarIntegrationRequest.md)
 - [UpdateDarSection200Response](docs/UpdateDarSection200Response.md)
 - [UpdateDarSection200ResponseData](docs/UpdateDarSection200ResponseData.md)
 - [UpdateDarTemplateRequest](docs/UpdateDarTemplateRequest.md)
 - [UpdateDataCustodianNetwork200Response](docs/UpdateDataCustodianNetwork200Response.md)
 - [UpdateDataProviderColl200Response](docs/UpdateDataProviderColl200Response.md)
 - [UpdateDataProviderCollRequest](docs/UpdateDataProviderCollRequest.md)
 - [UpdateDatasetsRequest](docs/UpdateDatasetsRequest.md)
 - [UpdateDur200Response](docs/UpdateDur200Response.md)
 - [UpdateDurIntegrations200Response](docs/UpdateDurIntegrations200Response.md)
 - [UpdateDurIntegrations200ResponseData](docs/UpdateDurIntegrations200ResponseData.md)
 - [UpdateFederationTeamRequest](docs/UpdateFederationTeamRequest.md)
 - [UpdateLicenses200Response](docs/UpdateLicenses200Response.md)
 - [UpdateProgrammingLanguages200Response](docs/UpdateProgrammingLanguages200Response.md)
 - [UpdateProgrammingLanguagesRequest](docs/UpdateProgrammingLanguagesRequest.md)
 - [UpdateProgrammingPackages200Response](docs/UpdateProgrammingPackages200Response.md)
 - [UpdatePublicationsRequest](docs/UpdatePublicationsRequest.md)
 - [UpdateQuestionBankQuestion200Response](docs/UpdateQuestionBankQuestion200Response.md)
 - [UpdateQuestionBankQuestionRequest](docs/UpdateQuestionBankQuestionRequest.md)
 - [UpdateQuestionBankQuestionStatus200Response](docs/UpdateQuestionBankQuestionStatus200Response.md)
 - [UpdateReviews200Response](docs/UpdateReviews200Response.md)
 - [UpdateReviews200ResponseData](docs/UpdateReviews200ResponseData.md)
 - [UpdateReviewsRequest](docs/UpdateReviewsRequest.md)
 - [UpdateTeamDarApplicationQuestionReview200Response](docs/UpdateTeamDarApplicationQuestionReview200Response.md)
 - [UpdateTeamDarApplicationRequest](docs/UpdateTeamDarApplicationRequest.md)
 - [UpdateToolsIntegrationsRequest](docs/UpdateToolsIntegrationsRequest.md)
 - [UpdateToolsRequest](docs/UpdateToolsRequest.md)
 - [UpdateTypeCategories200Response](docs/UpdateTypeCategories200Response.md)
 - [UpdateTypeCategoriesRequest](docs/UpdateTypeCategoriesRequest.md)
 - [UpdateUserHasRolesRequest](docs/UpdateUserHasRolesRequest.md)
 - [UpdateUserHasRolesRequestRoles](docs/UpdateUserHasRolesRequestRoles.md)
 - [UpdateWidget200Response](docs/UpdateWidget200Response.md)
 - [UpdateWidgetRequest](docs/UpdateWidgetRequest.md)
 - [UploadDurRequest](docs/UploadDurRequest.md)
 - [User](docs/User.md)
 - [VerifySecondaryEmail200Response](docs/VerifySecondaryEmail200Response.md)
 - [VerifySecondaryEmail400Response](docs/VerifySecondaryEmail400Response.md)
 - [VerifySecondaryEmail404Response](docs/VerifySecondaryEmail404Response.md)
 - [Widget](docs/Widget.md)
 - [WidgetAnalytics200Response](docs/WidgetAnalytics200Response.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="bearerAuth"></a>
### bearerAuth

- **Type**: Bearer authentication (JWT)

