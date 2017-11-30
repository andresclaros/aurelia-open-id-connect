
**Aurelia OpenID Connect** is a distrubuted authorization and authentication plugin for Aurelia. It works as an adapter to the popular open-source [oidc-client-js package from IdentityModel][oidc-client-js]. This blog post commemorates the 1.0.0 release of the Aurelia OpenID Connect plugin. 

The Aurelia OpenID Connect plugin adds distributed authentication and authorization capacities to an app. Whereas authentication testifies to the end-user's identity, authorization testifies to what the end-user can access. [OpenID Connect][open-id-connect] is an internet standard. It extends OAuth's authorization capacities with OpenID's identity capacities. As such, OpenID Connect lets an application answer two questions about its end-users: Who are you? What can you access?

The Aurelia OpenID Connect plugin is an adapter to the standard-compliant oidc-client-js package. It is possible to use oidc-client-js on its own. What the Aurelia plugin provides is 1. integration with the Aurelia router, 2. a login/logout component, 3. a navigation filter, and 4. a way to observe the state of the end-user.

The 1.0 release of the Aurelia OpenID Connect plugin is ready for consumption in production applications. It has > 95% test coverage, 28 GitHub stars, 34 closed issues (19 are external issues), and several demos in two repositories. The plugin's public API has stabilized, and from the 1.0 release forward, we will follow the [Semantic Versioning][semver] rules around breaking changes. 

What follows are a few resource to help you get started. Pull requests and issues are most welcome! 

https://github.com/shaunluttin/aurelia-open-id-connect

* This is the plugin's source-code repository. 
* The README.md contains usage instructions. 

https://github.com/shaunluttin/aurelia-open-id-connect-demos 

* This repository contains official demos. 
* Currently, the demos include a pure client-side app and an app that integrates ASP.NET Core server-side rendering. 
* The demos use OpenID Connect with these providers: 
  * Azure Active Directory. 
  * Auth0
  * Identity Server

https://github.com/openiddict/openiddict-samples/tree/dev/samples/ImplicitFlow 

* This is a demo/sample repository for OpenIddict. 
* There is a LIVE version of this demo here: http://zamboni-app.azurewebsites.net/ 
* The implicit flow sample uses an Aurelia client application, two ASP.NET Core Resource Servers, and an ASP.NET Core OpenID Connect Provider. 

[oidc-client-js]: https://github.com/IdentityModel/oidc-client-js

[open-id-connect]: http://openid.net/connect/

[semver]: https://semver.org/
