# The-M-Project generator [![Build Status](https://travis-ci.org/mwaylabs/generator-tmp2.png)](https://travis-ci.org/mwaylabs/generator-tmp2)

A [Yeoman](http://yeoman.io) generator for [The-M-Project](http://the-m-project.org).

## Notice
This module is under development and not yet ready for production use.

## Getting Started

Make sure you have installed Node.js, Git and optionally, Ruby and Compass (if you plan to use Compass).

Install: `npm install -g generator-tmp2`

Make a new directory and `cd` into it:
```bash
mkdir my-new-project && cd $_
```

Run `yo tmp2`, optionally passing an app name:
```bash
yo tmp2 [app-name]
```

Run `grunt` for building and `grunt server` for preview

## Generators

Available generators:

* [tmp2](#app)
* [tmp2:view](#view)
* [tmp2:layout](#layout)
* [tmp2:controller](#controller)
* [tmp2:model](#model)
* [tmp2:collection](#collection)
* [tmp2:router](#router)
* [tmp2:i18n](#i18n)

### App
Create a new The-M-Project app and generate all the boilerplate for you.

```bash
yo tmp2
```

### View

Generates a view in `app/scripts/views`.

Example:
```bash
yo tmp2:view profile
```

Produces `app/scripts/views/profile.js`:

```javascript
APPNAME.Views.ProfileView = M.View.extend({
   // ...
})
```
### Layout

Generates a layout in `app/scripts/layouts`.

Example:
```bash
yo tmp2:layout custom
```

Produces `app/scripts/layouts/custom.js`:

```javascript
APPNAME.Layouts.CustomLayout = M.Layout.extend({
   // ...
})
```

### Controller

Generates a controller in `app/scripts/controllers`.

Example:
```bash
yo tmp2:controller register
```

Produces `app/scripts/controllers/register.js`:

```javascript
APPNAME.Controllers.RegisterController = M.Controller.extend({
   // ...
})
```

### Model

Generates a model in `app/scripts/models`.

Example:
```
yo tmp2:model user
```

Produces `app/scripts/models/user.js`:

```
APPNAME.Models.UserModel = M.Model.extend({
   // ...
})
```

### Collection

Generates a collection in `app/scripts/collections`.

Example:
```bash
yo tmp2:collection user
```

Produces `app/scripts/collections/user.js`:

```javascript
APPNAME.Collections.UserCollection = M.Collection.extend({
   // ...
})
```

### Router

Generates a router in `app/scripts/routers`.

Example:
```bash
yo tmp2:routers myRouter
```

Produces `app/scripts/routers/myRouter.js`:

```javascript
APPNAME.Routers.MyrouterRouter = M.Router.extend({
   // ...
})
```

### I18N

Generates a i18n in `app/i18n`.

Example:
```bash
yo tmp2:i18n en
```

Produces `app/i18n/en.json`:

```javascript
{
    "global.button.save": "Save document",
    "global.button.emptyTrash": "Empty Trash ({{count}})",
    "global.error.permissionDenied": "Permission denied"
}
```

## Options

* `--skip-install`

  Skips the automatic execution of `bower` and `npm` after scaffolding has finished.

* `--test-framework <framework>`

  Defaults to `mocha`. Can be switched for another supported testing framework like `jasmine`.


## Contribute

See the [contributing docs](https://github.com/yeoman/yeoman/blob/master/contributing.md)

When submitting an issue, please follow the [guidelines](https://github.com/yeoman/yeoman/blob/master/contributing.md#issue-submission). Especially important is to make sure Yeoman is up-to-date, and providing the command or commands that cause the issue.

When submitting a bugfix, write a test that exposes the bug and fails before applying your fix. Submit the test alongside the fix.

When submitting a new feature, add tests that cover the feature.

## License

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
