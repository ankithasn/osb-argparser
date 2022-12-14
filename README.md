# Go API client for swagger

The Open Service Broker API defines an HTTP(S) interface between Platforms and Service Brokers.

## Overview
This API client was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project.  By using the [swagger-spec](https://github.com/swagger-api/swagger-spec) from a remote server, you can easily generate an API client.

- API version: master - might contain changes that are not yet released
- Package version: 1.0.0
- Build package: io.swagger.codegen.v3.generators.go.GoClientCodegen
For more information, please visit [https://www.openservicebrokerapi.org/](https://www.openservicebrokerapi.org/)

## Installation
Put the package under your project folder and add the following in import:
```golang
import "./swagger"
```

## Documentation for API Endpoints

All URIs are relative to *http://example.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CatalogApi* | [**CatalogGet**](docs/CatalogApi.md#catalogget) | **Get** /v2/catalog | get the catalog of services that the service broker offers
*ServiceBindingsApi* | [**ServiceBindingBinding**](docs/ServiceBindingsApi.md#servicebindingbinding) | **Put** /v2/service_instances/{instance_id}/service_bindings/{binding_id} | generate a service binding
*ServiceBindingsApi* | [**ServiceBindingGet**](docs/ServiceBindingsApi.md#servicebindingget) | **Get** /v2/service_instances/{instance_id}/service_bindings/{binding_id} | get a service binding
*ServiceBindingsApi* | [**ServiceBindingLastOperationGet**](docs/ServiceBindingsApi.md#servicebindinglastoperationget) | **Get** /v2/service_instances/{instance_id}/service_bindings/{binding_id}/last_operation | get the last requested operation state for service binding
*ServiceBindingsApi* | [**ServiceBindingUnbinding**](docs/ServiceBindingsApi.md#servicebindingunbinding) | **Delete** /v2/service_instances/{instance_id}/service_bindings/{binding_id} | deprovision a service binding
*ServiceInstancesApi* | [**ServiceInstanceDeprovision**](docs/ServiceInstancesApi.md#serviceinstancedeprovision) | **Delete** /v2/service_instances/{instance_id} | deprovision a service instance
*ServiceInstancesApi* | [**ServiceInstanceGet**](docs/ServiceInstancesApi.md#serviceinstanceget) | **Get** /v2/service_instances/{instance_id} | get a service instance
*ServiceInstancesApi* | [**ServiceInstanceLastOperationGet**](docs/ServiceInstancesApi.md#serviceinstancelastoperationget) | **Get** /v2/service_instances/{instance_id}/last_operation | get the last requested operation state for service instance
*ServiceInstancesApi* | [**ServiceInstanceProvision**](docs/ServiceInstancesApi.md#serviceinstanceprovision) | **Put** /v2/service_instances/{instance_id} | provision a service instance
*ServiceInstancesApi* | [**ServiceInstanceUpdate**](docs/ServiceInstancesApi.md#serviceinstanceupdate) | **Patch** /v2/service_instances/{instance_id} | update a service instance

## Documentation For Models

 - [AsyncOperation](docs/AsyncOperation.md)
 - [Catalog](docs/Catalog.md)
 - [Context](docs/Context.md)
 - [DashboardClient](docs/DashboardClient.md)
 - [LastOperationResource](docs/LastOperationResource.md)
 - [MaintenanceInfo](docs/MaintenanceInfo.md)
 - [Metadata](docs/Metadata.md)
 - [ModelError](docs/ModelError.md)
 - [Object](docs/Object.md)
 - [Plan](docs/Plan.md)
 - [Schemas](docs/Schemas.md)
 - [Service](docs/Service.md)
 - [ServiceBindingEndpoint](docs/ServiceBindingEndpoint.md)
 - [ServiceBindingMetadata](docs/ServiceBindingMetadata.md)
 - [ServiceBindingRequest](docs/ServiceBindingRequest.md)
 - [ServiceBindingResouceObject](docs/ServiceBindingResouceObject.md)
 - [ServiceBindingResource](docs/ServiceBindingResource.md)
 - [ServiceBindingResponse](docs/ServiceBindingResponse.md)
 - [ServiceBindingSchema](docs/ServiceBindingSchema.md)
 - [ServiceBindingVolumeMount](docs/ServiceBindingVolumeMount.md)
 - [ServiceBindingVolumeMountDevice](docs/ServiceBindingVolumeMountDevice.md)
 - [ServiceInstanceAsyncOperation](docs/ServiceInstanceAsyncOperation.md)
 - [ServiceInstanceMetadata](docs/ServiceInstanceMetadata.md)
 - [ServiceInstancePreviousValues](docs/ServiceInstancePreviousValues.md)
 - [ServiceInstanceProvisionRequestBody](docs/ServiceInstanceProvisionRequestBody.md)
 - [ServiceInstanceProvisionResponse](docs/ServiceInstanceProvisionResponse.md)
 - [ServiceInstanceResource](docs/ServiceInstanceResource.md)
 - [ServiceInstanceSchema](docs/ServiceInstanceSchema.md)
 - [ServiceInstanceSchemaCreate](docs/ServiceInstanceSchemaCreate.md)
 - [ServiceInstanceUpdateRequestBody](docs/ServiceInstanceUpdateRequestBody.md)

## Documentation For Authorization

## basicAuth
- **Type**: HTTP basic authentication

Example
```golang
auth := context.WithValue(context.Background(), sw.ContextBasicAuth, sw.BasicAuth{
	UserName: "username",
	Password: "password",
})
r, err := client.Service.Operation(auth, args)
```

## Author

open-service-broker-api@googlegroups.com
