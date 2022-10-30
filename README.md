# AceLords Laravel 5, 6 & 7 Skeleton Project 

An AceLords skeleton project for kick-starting other projects. 
Forms a good place to kickstart development instead of starting from scratch.
> Made with Vue.js and Modular in design.

### In a Nutshell
- [Laravel ^6](https://laravel.com/)
- [Vue ^2](https://vuejs.org)
- Redis
- Laravel Passport (API Authentication -> OAUTH2)
- Separated concerns between logic and vue templates (presentation layer). 
Easier for swapping an entire dashboard template without affecting the logic
- SASS
- [Vuetify v2](https://vuetifyjs.com/)
- [Tailwind](https://tailwindcss.com/)
- [Laravel Envoy](https://laravel.com/docs/master/envoy) (zero-downtime deployment into production)
- No migrations. Instead, a MySQl workbench file is provided
- SEO-ready
- Login with either username, email, or phone number


## Modules
- **Blog** (posts, categories, tags, blog uploads)
- **Emails** (Inbound and outbound emails)
- **Settings** (redis, horizon, system configurations, domain settings, organization, policy pages, SEO, `.env` mgmt)
- **SMS** (Nexmo, AfricasTalking, OTP)
- **Users** (users, roles & permissions, manage accounts, notifications, login info, departments, account issues)


## Demo

The demo will be up in the specified domain
- [AceLords Website](https://skeleton.acelords.com)
> Admin Login info: 
>
> Username: acelords
>
> Password: acelords

## Donating to the project
If you've found this useful and would like to buy the maintainers a coffee (or a Tesla, we're not picky), feel free to do so.


#### Crowdfunding

**DONATE:** If this project helped you or your business in any way and you feel like donating some change, you can always buy me a cup of coffee :)

<a href="https://ko-fi.com/acelords" target="_blank" title="Buy me a Coffee"><img width="150" style="border:0px;width:150px;display:block;margin:0 auto" src="https://az743702.vo.msecnd.net/cdn/kofi2.png?v=0" border="0" alt="Buy Me a Coffee at ko-fi.com" /></a>

Or by buying products and merchandise at [Marketplace](https://store.acelords.com).

This funding is used for maintaining the project and adding new features into Code Style plus other open-source repositories.

> NB: Some donations will also go to support the creators listed under **Special Thanks** section. They have done an incredible job
> that needs to be rewarded as much as possible.


#### Special thanks
During the development of this dashboard, we have used many existing resources from awesome developers. We want to thank them for providing their tools open source:
- [Vuetify](https://vuetifyjs.com/en/) for the wonderful framework
- [Core UI](https://coreui.io) for the wonderful vue admin dashboard

Let us know your thoughts below. And good luck with development!

## Screenshots
![Dashboard](https://github.com/acelords/skeleton/blob/master/screenshot1.png)

![Dashboard 2](https://github.com/acelords/skeleton/blob/master/screenshot2.png)

![Dashboard 3](https://github.com/acelords/skeleton/blob/master/screenshot3.png)

![Dashboard 4](https://github.com/acelords/skeleton/blob/master/screenshot4.jpg)

![Dashboard 5](https://github.com/acelords/skeleton/blob/master/screenshot5.jpg)

![Dashboard 6](https://github.com/acelords/skeleton/blob/master/screenshot6.jpg)

## Vuetify
Vuetify is developed exactly according to Material Design spec. Every component is hand crafted to bring you the best possible UI tools to your next great app. The development doesn't stop at the core components outlined in Google's spec. Through the support of community members and sponsors, additional components will be designed and made available for everyone to enjoy.


## Vuex

Vuex is a state management pattern + library for Vue.js applications. It serves as a centralized store for all the components in an application, with rules ensuring that the state can only be mutated in a predictable fashion. It also integrates with Vue's official [devtools](https://github.com/vuejs/vue-devtools) extension to provide advanced features such as zero-config time-travel debugging and state snapshot export / import.

## Laravel Mix
Bundling is done by [Laravel Mix](https://laravel.com/docs/6.x/mix)

## Documentation
The documentation for the project is hosted at our [website](https://skeleton.acelords.com). 
> NB: Coming soon


## File Structure

Within the project you'll find the following directories and files:

> NB: All files could not be captured in this section, but the files and folders captured here
>represent the general pattern used in the project.

```
acelords-skeleton
├── CHANGELOG.md
├── LICENSE
├── README.md
├── DEVELOPER.md
├── DEVELOPER-SNIPPETS.md
├── babel.config.js
├── cypress.json
├── jest.config.js
├── package.json
├── postcss.config.js
├── vue.config.js
├── webpack.config.js
├── webpack.mix.js
├── app
│   ├── Console
│   │   └── Commands
│   ├── Exceptions
│   ├── Http
│   │   ├── Controllers
│   │   │   ├── ContactMessagesController.php
│   │   │   ├── Controller.php
│   │   │   ├── MediaController.php
│   │   │   ├── PagesController.php
│   │   │   └── WidgetController.php
│   │   ├── Middleware
│   │   │   ├── Authenticate.php
│   │   │   ├── CheckForMaintenanceMode.php
│   │   │   ├── EncryptCookies.php
│   │   │   ├── RedirectIfAuthenticated.php
│   │   │   ├── TrimStrings.php
│   │   │   ├── TrustProxies.php
│   │   │   └── VerifyCsrfToken.php
│   │   └── Kernel.php
│   ├── Library
│   │   ├── Contracts
│   │   │   └── WidgetsInerface.php
│   │   ├── Facades
│   │   │   └── Uploader.php
│   │   ├── Helpers
│   │   │   └── helpers.php
│   │   ├── Modules
│   │   │   ├── Blog
│   │   │   ├── Emails
│   │   │   ├── Settings
│   │   │   ├── Users
│   │   │   └── Foo
│   │   │       ├── Config
│   │   │       │   ├── events.php
│   │   │       │   ├── laratrust.php
│   │   │       │   ├── settings.php
│   │   │       │   └── sidebar.php
│   │   │       ├── Contracts
│   │   │       ├── Decorators
│   │   │       ├── Events
│   │   │       ├── Facades
│   │   │       ├── Http
│   │   │       │   ├── Controllers
│   │   │       │   ├── Filters
│   │   │       │   ├── Requests
│   │   │       │   └── Resources
│   │   │       ├── Jobs
│   │   │       ├── Listeners
│   │   │       ├── Mail
│   │   │       ├── Models
│   │   │       ├── Notifications
│   │   │       ├── Repositories
│   │   │       ├── Routes
│   │   │       ├── Services
│   │   │       └── Traits
│   │   │       └── Widgets
│   │   ├── Repositories
│   │   │   └── ModuleRepository.php
│   │   ├── Services
│   │   │   └── UploaderService.php
│   │   ├── Traits
│   │   │   ├── Encryptable.php
│   │   │   ├── FetchAllDatabaseTablesTrait.php
│   │   │   ├── PermissionsGeneratorTrait.php
│   │   │   ├── QueueMailConstants.php
│   │   │   ├── ThemesTrait.php
│   │   │   └── WidgetsTrait.php
│   │   ├── Widgets
│   │   │   ├── PolicyPage.php
│   │   │   └── WidgetsEvaluator.php
│   │   └── Widgetifier.php
│   ├── Models
│   │   ├── ContactMessage.php
│   │   └── Upload.php
│   └── Providers
│       ├── AppServiceProvider.php
│       ├── AuthServiceProvider.php
│       ├── BroadcastServiceProvider.php
│       ├── EventServiceProvider.php
│       ├── HorizonServiceProvider.php
│       ├── ProjectEventServiceProvider.php
│       ├── ProjectFrontendRouteServiceProvider.php
│       ├── ProjectRouteServiceProvider.php
│       ├── ProjectServiceProvider.php
│       └── RouteServiceProvider.php
├── bootstrap
├── config
├── database
│   └── project.mwb
├── public
│   ├── favicon.ico
│   ├── css
│   ├── img
│   ├── js
│   ├── logos
│   ├── favicons
│   ├── vendor
│   ├── fonts
│   └── index.php
├── resources
│   ├── js
│   │   ├── components
│   │   │   ├── passport
│   │   │   │   ├── AuthorizedClients.vue
│   │   │   │   ├── Clients.vue
│   │   │   │   └── PersonalAcccessTokens.vue
│   │   │   └── widgets
│   │   ├── libs
│   │   ├── modules
│   │   │   ├── core
│   │   │   ├── settings
│   │   │   └── users
│   │   │       ├── libs
│   │   │       │   ├── departments
│   │   │       │   │   ├── Department.js
│   │   │       │   │   └── DepartmentRepository.js
│   │   │       │   ├── notifications
│   │   │       │   │   └── Notification.js
│   │   │       │   ├── permissions
│   │   │       │   ├── profiles
│   │   │       │   ├── logins
│   │   │       │   └── users
│   │   │       │       ├── loginMixin.js
│   │   │       │       ├── User.js
│   │   │       │       ├── userLoggedInMixin.js
│   │   │       │       ├── UserRepository.js
│   │   │       │       └── usersMixin.js
│   │   │       └── paths.js
│   │   ├── plugins
│   │   │   ├── chartist.js
│   │   │   ├── icons.js
│   │   │   └── vuetify.js
│   │   ├── store
│   │   ├── templates
│   │   │   ├── vuetifycoreui
│   │   │   │   └── js
│   │   │   │       ├── components
│   │   │   │       │   ├── admin
│   │   │   │       │   ├── core
│   │   │   │       │   │   ├── Dashboard.vue
│   │   │   │       │   │   └── routes.js
│   │   │   │       │   ├── layouts
│   │   │   │       │   ├── material
│   │   │   │       │   ├── settings
│   │   │   │       │   └── users
│   │   │   │       │       ├── departments
│   │   │   │       │       │   └── Index.vue
│   │   │   │       │       ├── notifications
│   │   │   │       │       │   ├── Drawer.vue
│   │   │   │       │       │   ├── Index.vue
│   │   │   │       │       │   └── List.vue
│   │   │   │       │       ├── permissions
│   │   │   │       │       ├── profiles
│   │   │   │       │       ├── logins
│   │   │   │       │       └── users
│   │   │   │       │           ├── Create.vue
│   │   │   │       │           ├── Edit.vue
│   │   │   │       │           ├── Index.vue
│   │   │   │       │           └── Show.vue
│   │   │   │       ├── paths.js
│   │   │   │       ├── routes.js
│   │   │   │       └── views.js
│   │   │   └── vuetifylaravel
│   │   └── utils
│   │       ├── Event.js
│   │       ├── filters.js
│   │       ├── inactivityGuard.js
│   │       ├── Permissions.js
│   │       ├── Settings.js
│   │       ├── titleMixin.js
│   │       ├── Util.js
│   │       └── vuex.js
│   ├── lang
│   ├── sass
│   │   ├── app.scss
│   │   ├── bootstrap.scss
│   │   ├── coreui.scss
│   │   ├── tailwind.scss
│   │   ├── vuebar.scss
│   │   ├── vuetify.scss
│   │   ├── vuetifycoreui.scss
│   │   └── vuetifylaravel.scss
│   └── views
│       ├── auth
│       ├── errors
│       ├── layouts
│       ├── templates
│       │   ├── vuetifycoreui
│       │   │   └── layouts
│       │   │       └── main.blade.php
│       │   └── vuetifylaravel
│       │       └── layouts
│       │           └── main.blade.php
│       └── vendor
├── routes
│   ├── api.php
│   ├── channels.php
│   ├── console.php
│   └── web.php
├── storage
│   ├── app
│   ├── framework
│   │   ├── cache
│   │   ├── sessions
│   │   ├── testing
│   │   └── views
│   └── logs
└── tests
    ├── e2e
    │   ├── plugins
    │   │   └── index.js
    │   ├── specs
    │   │   └── test.js
    │   └── support
    │       ├── commands.js
    │       └── index.js
    ├── Feature
    └── Unit
```

## Browser Support

At present, we officially aim to support the last two versions of the following browsers:

<img src="https://s3.amazonaws.com/creativetim_bucket/github/browser/chrome.png" width="64" height="64"> <img src="https://s3.amazonaws.com/creativetim_bucket/github/browser/firefox.png" width="64" height="64"> <img src="https://s3.amazonaws.com/creativetim_bucket/github/browser/edge.png" width="64" height="64"> <img src="https://s3.amazonaws.com/creativetim_bucket/github/browser/safari.png" width="64" height="64"> <img src="https://s3.amazonaws.com/creativetim_bucket/github/browser/opera.png" width="64" height="64">


## Reporting Issues
We use Gitlab and/or Github Issues as the official bug tracker for the project. Here are some advices for our users that want to report an issue:

1. Make sure that you are using the latest version of the Vuetify Material Dashboard.
2. Providing us reproducible steps for the issue will shorten the time it takes for it to be fixed.
3. Some issues may be browser specific, so specifying in what browser you encountered the issue might help.

## Technical Support or Questions

If you have questions or need help integrating the product please [contact us](https://acelords.com) instead of opening an issue.

## Licensing

- Copyright 2019 AceLords (https://www.acelords.com)

## Useful Links

- [More products](https://store.acelords.com) from AceLords Store/Marketplace

##### Social Media

Twitter: <https://twitter.com/AceLords>

Facebook: <https://www.facebook.com/acelords.com>

Instagram: <https://instagram.com/acelords>

![AceLords](https://github.com/acelords/skeleton/blob/master/AceLords_skeleton_brand_minilogo.png)
