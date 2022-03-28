---
title:  Liquit Workspace - Identities
#tags: [Liquit Workspace, Application Delivery]
keywords: Managed Application Delivery Services, MAD, Liquit Workspace
#last_updated: March 3, 2022
#summary: "Collections are useful if you want to loop through a special folder of pages that you make available in a content API. You could also use collections if you have a set of articles that you want to treat differently from the other content, with a different layout or format."
sidebar: managed_application_delivery_services-sidebar
permalink: mad_liquit_workspace_identities.html
folder: managed_application_delivery_services
---


Source documentation: [Contexts - Identities](https://docs.liquit.com/docs/lws-identities-contexts), [Device Collections - Identities](https://docs.liquit.com/docs/lws-identities-device-collections),[Devices - Identities](https://docs.liquit.com/docs/lws-identities-devices), [Groups - Identities](https://docs.liquit.com/docs/lws-identities-groups) and [Users - Identities](https://docs.liquit.com/docs/lws-identities-users)

 
## Contexts

A Context basically is a group of filters which determine which objects are a member of the Context, these filters can include but are not limited to location filters and LDAP attributes. They allow you to assign Variables, Packages, Access Policies and Deployments dynamically. This feature comes in handy when you want to restrict access based on certain attributes.

A context object has access to filters based on the device, session and user objects. Even a scripting option is available to create complex contexts which can’t be solved with the editor. Context awareness in Liquit Workspace 3.0 allows you to:

> Publish applications based on the department field as configured within your Active Directory.
> Combine information about a device and user to assign applications, so only if User A is logged on Device B will grant him access to the application.
> By assigning Liquit permissions to contexts allows you to only have Administrative access to the Liquit Workspace from within the company network, any other location will give normal user permissions.

### Context settings

In the following chapters the settings within a context will be described
#### Overview

In the overview General Settings are configured. 
#### Filters

Filters are only available to you if you chose to create a filter type Context. The filters enable you to define the attributes that define the Context.

You can find additional information in the following link [Context Filters - Filters](https://docs.liquit.com/docs/lws-appendix-filters-context-filters).
#### Devices

Shows a list of possible devices that can be assigned the context. User-based filters are ignored when showing this list.
#### Variables

Contexts let you override system wide variables and let you define completely new variables. To override an existing variable simply click the variable and enter a new value for the variable. To add a new one click the “Add Variable” button and enter your new key value pair. 

You can find additional information in the following link [Variables - Appendix](https://docs.liquit.com/docs/lws-appendix-variables).

{% include note.html content="Variables are not applied on the windows environment. The variables are only used in the Liquit workspace processes." %}

#### Access Policy

It is possible to assign “Access Policies” to contexts, this allows for advanced scenario’s. You can for example assign different policies to users connecting to the Liquit Workspace from a certain IP Address. To assign an access policy you need to create it first. 

{% include note.html content="The liquit as a Service services are cloud hosted. Remember to use the public IP-adress to define a company network." %}

You can find additional information in the following link [Liquit Workspace - System](https://loginconsultants.atlassian.net/wiki/spaces/orangeworkspace/pages/2028994599) and [Access Policies - System](https://docs.liquit.com/docs/lws-system-access-policies).
#### Content Access

N/A
#### Portal Settings

The portal settings tab allows you to override the portal settings for the given context. 

You can find additional information in the following link [Portal Settings - Portal](https://docs.liquit.com/docs/lws-portal-portal-settings).
#### User Settings

The user settings tab allows you to override the portal settings for the given context.

You can find additional information in the following link [User Settings - Portal](https://docs.liquit.com/docs/lws-portal-user-settings).
#### Login Settings

The login settings tab allows you to override the login settings for the given context.

You can find additional information in the following link [Login Settings - Portal](https://docs.liquit.com/docs/lws-portal-login-settings). 

{% include note.html content="Setting the login settings was not applied during testing. This needs to be investigated and retested. " %}
#### Packages

Packages can be assigned to contexts, to add a package simply use the lookup field and select it. The modal window presented will ask you how to assign the entitlement and which events should be used to initiate the package. 

You can find additional information in the following link [Packages - Workspace](https://docs.liquit.com/docs/lws-workspace-packages)
####  Deployments

Deployments can be assigned to contexts. To add a deployment you can use the lookup field.

You can find additional information in the following link [Deployments - Automation](https://docs.liquit.com/docs/lws-automation-deployments) and [Liquit Workspace - Automation](https://loginconsultants.atlassian.net/wiki/spaces/orangeworkspace/pages/2028994575)

{% include note.html content="Deployments needs to be approved by assignments. A deployment can be dynamically assigned with contexts.
Different types of contexts." %}


> DTAP contexts
    > Production contexts
    > Acceptance contexts
    > Test contexts
> Filter contexts (A filter context is used to query devices based on all devices. For example, a filter context is used to filter all devices with a liquit agent with version X. )

#### Contexts conflicting settings

It is possible to have multiple contexts applied to the user environment. Conflicts are able to apply if multiple contexts are applied. The following table describes the actions take during conflicts.

Context Settings | Priority with conflicting contexts
Variables | Lowest priority if variable is 
Access Policy | Highest amount rights is applied
Content Access | Unknown - Need testing
Portal Settings | Lowest priority if settings is configured
User Settings | Highest priority if settings is configured
Login Settings | Unknown - No settings applied during testing. General settings always prevailed
Packages | All package assignments are applied
Deployments | All deployments are approved

See the chapter [Design Decissions](mad_liquit_workspace_designdecisions.md) for the design decisions.

#### Device Collections

Device Collections are groups for your devices, they allow you to add devices to a collection.
This feature comes in handy when you want to manage a group of devices, for example when you want to run a certain action on a selection of devices.

Dynamically grouping devices based on attributes and more could by achieved by using the Contexts feature.
#### Devices

Devices are a list of Devices that have been connected to your Liquit Workspace.
They allow you to assign Packages and Deployments to defined Devices, you can also view users who currently logged in on a Device. Currently it is required for the Device to have an Agent running to be registered.
#### Groups

Groups are available from added Identity Sources, it currently is not possible to add, remove or edit any groups. However it is possible to assign Packages and Access Polices to them.
#### Users

Users are available from added Identity Sources and from the LOCAL identity source, currently it is only possible to add, remove users within the LOCAL identity source. However it is possible to assign different entities to them.

See the chapter [Design Decissions](mad_liquit_workspace_designdecisions.md) for the design decisions.