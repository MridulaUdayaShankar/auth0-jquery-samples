# Auth0 jQuery Embedded Login

This sample demonstrates how to add authentication to a jQuery application using Auth0's Lock widget.

## Getting Started

If you haven't already done so, [sign up](https://auth0.com) for your free Auth0 account and create a new client in the [dashboard](https://manage.auth0.com). Find the **domain** and **client ID** from the settings area and add the URL for your application to the **Allowed Callback URLs** box. If you are serving the application with the provided `serve` library, that URL is `http://localhost:5000`.

Clone the repo or download it from the JavaScript quickstart page in Auth0's documentation.

```bash
cd 01-Embedded-Login
npm install
```

## Set the Client ID and Domain 

To configure the application for your Auth0 account settings, rename the `auth0-variables.js.example` file to `auth0-variables.js` and provide the **client ID** and **domain** there. 

## Enable Cross Origin Authentication

In order to be able to log-in with user and password you need to enable the [Cross Origin Authentication](https://auth0.com/docs/cross-origin-authentication). This is not required for Social or Enterprise connections.

Make sure you edit the contents of the `callback-cross-auth.html` file to match your **client Id**, **domain** and **callback** settings. This page will only be used when third-party cookies are disabled in certain browsers, and *needs to be served over HTTPS*. Note that when third-party cookies are disabled, there are some browsers where the authentication flow will NOT work. 

## Run the Application

The `serve` module provided with this sample can be run with the `start` command.

```bash
npm start
```

The application will be served at `http://localhost:5000`.

## What is Auth0?

Auth0 helps you to:

* Add authentication with [multiple authentication sources](https://docs.auth0.com/identityproviders), either social like **Google, Facebook, Microsoft Account, LinkedIn, GitHub, Twitter, Box, Salesforce, amont others**, or enterprise identity systems like **Windows Azure AD, Google Apps, Active Directory, ADFS or any SAML Identity Provider**.
* Add authentication through more traditional **[username/password databases](https://docs.auth0.com/mysql-connection-tutorial)**.
* Add support for **[linking different user accounts](https://docs.auth0.com/link-accounts)** with the same user.
* Support for generating signed [Json Web Tokens](https://docs.auth0.com/jwt) to call your APIs and **flow the user identity** securely.
* Analytics of how, when and where users are logging in.
* Pull data from other sources and add it to the user profile, through [JavaScript rules](https://docs.auth0.com/rules).

## Create a free Auth0 account

1. Go to [Auth0](https://auth0.com/signup) and click Sign Up.
2. Use Google, GitHub or Microsoft Account to login.

## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## Author

[Auth0](auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](LICENSE.txt) file for more info.


