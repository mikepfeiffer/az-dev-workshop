# Lab 2 - Add Sign-in to an ASP.NET Core Web App

1. Sign in to the Azure portal.
2. Navigate to the Azure AD App registrations page.
3. Select New registration.
4. When the Register an application page appears, enter your application's registration information, enter a meaningful application name that will be displayed to users of the app.
5. In Redirect URI, add `https://localhost:44321/` and select Register.
6. After registration, select the Authentication menu, and then add the following information:
* In Redirect URIs, add `https://localhost:44321/signin-oidc` and select Save.
* In the Advanced settings section, set Logout URL to `https://localhost:44321/signout-oidc`.
* Under Implicit grant, check ID tokens.
* Select Save.
7. Run the application to validate that it works


### Lifelines:

* [Add sign-in with Microsoft to an ASP.NET Core web app](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-v2-aspnet-core-webapp)

### Navigation:

* [Back to Lab Index](https://github.com/mikepfeiffer/az-dev-workshop)
