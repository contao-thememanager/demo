# Contao ThemeManager Demo
____

## About

This is the official demo for the Contao ThemeManager
In this demo website, you will get a few preconfigured articles that are built using the CTM framework.

Visit the [Documentation][docs] to learn about installing this demo.

## Table of contents

- [Versions](#versions)
- [Installation](#installation)
- [Documentation](#documentation)
- [Bugs and feature requests](#bugs-and-feature-requests)
- [License](#license)
- [Sponsoring](#sponsoring)

## Versions
This demo is maintained for the current long term support and the newest version for Contao.

See the [Contao release plan][contao-releaseplan] for details. Each demo version has a separate branch in this Git 
repository.

## Installation
The demo website can be installed alongside Contao, either through the Contao Manager or with [Composer][composer] on 
the command line.

### Via contao-manager
When installing a fresh Contao application, select Contao Theme and upload following demo file:

![Select the contao theme option and upload the file](/docs/_images/install/cm/selectTheme.png "Select Theme")


Type in
> contao-thememanager/demo

within the searchbar (**B**) and install it from the recommended themes using the latest version (5.2)

or

select the option 'Contao Theme' and upload the following file

| Contao Version |           Download            |
|----------------|:-----------------------------:|
| `5.2`          | [💾](/docs/demo/ctm-demo.zip) |


![Check the dependencies and install the theme](/docs/_images/install/cm/dependencies.png "Composer dependencies")
Install the theme and follow the usual contao setup


![This demo does not have an admin account thus you can create one in the setup wizard](/docs/_images/install/cm/account.png "Creating an account")
This demo does not deliver an admin account, so you can set your own credentials


### Via composer
This repository functions as a _Composer project_. You can install a full Contao application and this demo using the 
`create-project` command. We're assuming here you are familiar with the command line and Composer and have a functioning 
PHP and webserver setup.

1. Run `composer create-project contao-thememanager/demo:5.2 your-new-website`
2. Connect the database e.g. through `DATABASE_URL` in your `.env.local` file.
3. Import the database backup using `php vendor/bin/contao-console contao:backup:restore`
4. Create an admin account using `php vendor/bin/contao-console contao:user:create`

## Documentation
A german documentation (WIP - work in progress) can be found by using the following link:
<a title="Documentation" href="https://docs.contao-thememanager.com"><strong>Documentation </strong></a>

## Bugs and feature requests
We appreciate your contributions when opening issues or requesting features. To help keep our issue list tidy, we may 
need to close issues if questions go unanswered.

### Bugs
If you think you have found a bug please follow these guidelines
1. Search for existing issues and check if your problem has already been reported
2. Check if you are using the latest version and if the issue has been fixed already
3. Provide a step-by-step tutorial on how to reproduce the issue in an isolated environment using only the Contao 
ThemeManager Core

### Feature requests
Feature requests are welcome. But take a moment to find out whether your idea fits with the scope and aims of the 
project. It's up to you to make a strong case to convince the project's developers of the merits of this feature. Please 
provide as much detail and context as possible.

## License
This demo is licensed under the AGPL-3.0 License

## Sponsoring
If you find this plugin useful, please consider [sponsoring us][sponsor] to help contribute to our time invested and to 
further development of this and other open source projects. 
Thank you for your support! - [Oveleon](https://www.oveleon.de).

[docs]: https://docs.contao-thememanager.com
[composer]: https://getcomposer.org
[contao-releaseplan]: https://to.contao.org/release-plan
[sponsor]: https://github.com/sponsors/oveleon
