# ![LOGO](logo.png) AzureDeploymentManager **flow**ground Connector

## Description

A generated **flow**ground connector for the AzureDeploymentManager API (version 2018-09-01-preview).

Generated from: https://api.apis.guru/v2/specs/azure.com/deploymentmanager/2018-09-01-preview/swagger.json<br/>
Generated at: 2019-05-07T17:38:04+03:00

## API Description

REST APIs for orchestrating deployments using the Azure Deployment Manager (ADM). See https://docs.microsoft.com/en-us/azure/azure-resource-manager/deployment-manager-overview for more information.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Gets an operation resource.

*Tags:* `Operations`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `api-version` - _required_ - The API version to use for this operation.

### Deletes an artifact source.

*Tags:* `ArtifactSources`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `artifactSourceName` - _required_ - The name of the artifact source.
* `api-version` - _required_ - The API version to use for this operation.

### Gets an artifact source.

*Tags:* `ArtifactSources`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `artifactSourceName` - _required_ - The name of the artifact source.
* `api-version` - _required_ - The API version to use for this operation.

### Creates or updates an artifact source.

> Synchronously creates a new artifact source or updates an existing artifact source.

*Tags:* `ArtifactSources`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `artifactSourceName` - _required_ - The name of the artifact source.
* `api-version` - _required_ - The API version to use for this operation.

### Deletes a rollout resource.

> Only rollouts in terminal state can be deleted.

*Tags:* `Rollouts`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `rolloutName` - _required_ - The rollout name.
* `api-version` - _required_ - The API version to use for this operation.

### Gets detailed information of a rollout.

*Tags:* `Rollouts`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `rolloutName` - _required_ - The rollout name.
* `api-version` - _required_ - The API version to use for this operation.
* `retryAttempt` - _optional_ - Rollout retry attempt ordinal to get the result of. If not specified, result of the latest attempt will be returned.

### Creates or updates a rollout.

> This is an asynchronous operation and can be polled to completion using the location header returned by this operation.

*Tags:* `Rollouts`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `rolloutName` - _required_ - The rollout name.
* `api-version` - _required_ - The API version to use for this operation.

### Stops a running rollout.

> Only running rollouts can be canceled.

*Tags:* `Rollouts`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `rolloutName` - _required_ - The rollout name.
* `api-version` - _required_ - The API version to use for this operation.

### Restarts a failed rollout and optionally skips all succeeded steps.

> Only failed rollouts can be restarted.

*Tags:* `Rollouts`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `rolloutName` - _required_ - The rollout name.
* `skipSucceeded` - _optional_ - If true, will skip all succeeded steps so far in the rollout. If false, will execute the entire rollout again regardless of the current state of individual resources. Defaults to false if not specified.
* `api-version` - _required_ - The API version to use for this operation.

### Deletes the service topology.

*Tags:* `ServiceTopologies`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `api-version` - _required_ - The API version to use for this operation.

### Gets the service topology.

*Tags:* `ServiceTopologies`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `api-version` - _required_ - The API version to use for this operation.

### Creates or updates a service topology.

> Synchronously creates a new service topology or updates an existing service topology.

*Tags:* `ServiceTopologies`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `api-version` - _required_ - The API version to use for this operation.

### Deletes the service.

*Tags:* `Services`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `serviceName` - _required_ - The name of the service resource.
* `api-version` - _required_ - The API version to use for this operation.

### Gets the service.

*Tags:* `Services`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `serviceName` - _required_ - The name of the service resource.
* `api-version` - _required_ - The API version to use for this operation.

### Creates or updates a service in the service topology.

> Synchronously creates a new service or updates an existing service.

*Tags:* `Services`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `serviceName` - _required_ - The name of the service resource.
* `api-version` - _required_ - The API version to use for this operation.

### Deletes the service unit.

*Tags:* `ServiceUnits`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `serviceName` - _required_ - The name of the service resource.
* `serviceUnitName` - _required_ - The name of the service unit resource.
* `api-version` - _required_ - The API version to use for this operation.

### Gets the service unit.

*Tags:* `ServiceUnits`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `serviceName` - _required_ - The name of the service resource.
* `serviceUnitName` - _required_ - The name of the service unit resource.
* `api-version` - _required_ - The API version to use for this operation.

### Creates or updates a service unit under the service in the service topology.

> This is an asynchronous operation and can be polled to completion using the operation resource returned by this operation.

*Tags:* `ServiceUnits`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `serviceTopologyName` - _required_ - The name of the service topology .
* `serviceName` - _required_ - The name of the service resource.
* `serviceUnitName` - _required_ - The name of the service unit resource.
* `api-version` - _required_ - The API version to use for this operation.

### Deletes the step.

*Tags:* `Steps`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `stepName` - _required_ - The name of the deployment step.
* `api-version` - _required_ - The API version to use for this operation.

### Gets the step.

*Tags:* `Steps`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `stepName` - _required_ - The name of the deployment step.
* `api-version` - _required_ - The API version to use for this operation.

### Creates or updates a rollout step with the given step properties.

> Synchronously creates a new step or updates an existing step.

*Tags:* `Steps`

#### Input Parameters
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group. The name is case insensitive.
* `stepName` - _required_ - The name of the deployment step.
* `api-version` - _required_ - The API version to use for this operation.

## License

**flow**ground :- Telekom iPaaS / azure-com-deploymentmanager-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
