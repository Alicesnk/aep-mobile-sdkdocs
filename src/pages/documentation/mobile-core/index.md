# Mobile Core

<InlineAlert variant="warning" slots="text"/>

As of **April 1, 2020**, Apple will no longer support the UIWebView API. To avoid any issues, ensure that you are using iOS SDK version 2.3.4 or later. For more information about the UIWebView API, see [UIWebView ](https://developer.apple.com/documentation/uikit/uiwebview).

Mobile Core is mandatory for all Adobe Experience Platform app implementations. Mobile Core contains a common set of functionality and frameworks, including Experience Cloud Identity services, data event hub, Rules Engine, reusable networking, and disk access routines. The following sections provide additional information about what is provided in the Mobile Core extension.

## Mobile Core generic APIs

The SDK provides core, extension-independent APIs to facilitate the event tracking of user screens, actions, and PII data. Events generated by these APIs are published to the SDK event hub and are available for use by extensions. For instance, when the Analytics extension is installed, all user actions and app screens event data is sent to the appropriate Analytics reporting endpoints.

For more information, please read the [Mobile Core API reference](api-reference.md).

## Configuration

The Configuration extension provides different APIs to set up the SDK's configuration settings. For more information, please read the documentation on the [Configuration extension](configuration/index.md).

## Identity

The Identity framework lets your app use Experience Cloud ID (ECID). Using ECIDs improves synchronization with Adobe and other customer identifiers. For more information, please read the documentation on the [Identity extension](identity/index.md).

## Lifecycle

The Lifecycle extension lets you access information about the app's sessions, including device information, app installation, app upgrades, session start and pause times, number of application launches, and additional context data. For more information on how to use the Lifecycle API, please read the documentation on the [Lifecycle extension](lifecycle/index.md).

## Rules Engine

Rules Engine looks for the interactions between users and their associated data and lets you trigger specified actions based on rules that you define. For more information, please read the documentation on the [Rules Engine](rules-engine/index.md).

## Signal

The Signal extension allows you to send data third-party endpoints via GET and POST requests. Signals are configured by using rules in the Data Collection UI. For more information, please read the documentation on the [Signal extension](signal/index.md).

## Platform Services

The interaction with native platforms is mainly built into the Platform Services layer, which is used across all the extensions. It also makes it easy for the apps to customize the behavior if needed. For more information, see [Platform Services](platform-services/index.md).

