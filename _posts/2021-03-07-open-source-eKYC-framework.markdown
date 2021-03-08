---
layout: post
title:  "Open Source eKYC Framework - eKYC Hub"
date:   2021-03-07 11:39:56 +0100
categories: foss ekyc oidc
---
The Identity First Tech community releases a free and open-source framework, called eKYC Hub, that implements the OpenID Connect for Identity Assurance specification and can be used by any Identity Provider to allow for exchange of verified user attributes with client applications.

The source code repository for the eKYC Hub application can be found at [https://github.com/identityfirst/eKYC-Hub](https://github.com/identityfirst/eKYC-Hub).

The eKYC Hub implements the OpenID Connect for Identity Assurance 1.0 which is published at [https://openid.net/specs/openid-connect-4-identity-assurance-1_0-ID2.html](https://openid.net/specs/openid-connect-4-identity-assurance-1_0-ID2.html). The framework allows for integration with eKYC data providers (verification services).

The released open-source code mainly provides the following:
1) Provides an integration layer between the IDP and the different verification services -  this allows for the user to verify different data attributes and store them within the Hub.
2) Provides an interface allowing clients to request and receive verified attributes from the Identity Provider using the standard OpenID Connect for Identity Assurance protocol.

![image OIDC eKYC](/assets/idv_hub.png)

In the repository, you can also find a demo client application as well as an example integration of the eKYC Hub with an open source Identity Provider - KeyCloak. You will need to have Docker installed to run the demo.

The eKYC Hub has been implemented with [Passbase](https://passbase.com/) - one of the easy-to-use verification services which provides an SDK and RESTful API for verifying end user data. Other providers can be used depending on requirements.

All provided code is open-source and available under the Apache 2.0 license. We welcome feedback as well as contributions to the framework.


