# How to Write a README

The README file has a [long tradition](http://catb.org/~esr/jargon/html/R/README-file.html) in software projects.
Its purpose is to serve as the entry point for everything you might want to know about the project.
You may not necessarily include all information, but you should at least link to it form the README.
Even if you are just dumping your code onto GitHub and don't plan to support the project for others, it should include a README file.

Traditionally README files are plain text.
Most projects typically use a text-based markup which renders nicely in GitHub.
[Markdown](https://en.wikipedia.org/wiki/Markdown) is the simplest and most readable when viewed as plain text.
[AsciiDoc](http://asciidoc.org/) and [reStructuredText](http://docutils.sourceforge.net/rst.html) are more powerful and have features such as admonitions and generated table of contents.

The following sections will list and describe the major top-level sections you might find in a README file.
You don't need to include every possible section in your read me file.

## Table of Contents

* [Project Name](#project-name)
* [Shields](#shields)
* [Logo/Icon/Banner](#logoiconbanner)
* [Download Badge](#download-badge)
* [Short Description](#short-description)
* [Table Of Contents Section](#table-of-contents-section)
* [Screen Shots](#screen-shots)
* [Feature List](#feature-list)
* [Requirements](#requirements)
* [Installation](#installation)
* [Configuration](#configuration)
* [Usage/Quick Start](#usagequick-start)
* [Documentation](#documentation)
* [Examples](#examples)
* [FAQ](#faq)
* [Troubleshooting](#troubleshooting)
* [Non-Goals](#nongoals)
* [Changes](#changes)
* [Contributing](#contributing)
* [Contributors/Credits](#contributorscredits)
* [Security Disclosure](#security-disclosure)
* [Donations](#donations)
* [Author(s)](#authors)
* [Support/Help](#supporthelp)
* [Community/Communication](#communitycommunication)
* [Commercial Support](#commercial-support)
* [Sponsors](#sponsors)
* [Projects Using X](#projects-using-x)
* [Disclaimer](#disclaimer)
* [Related Projects](#related-projects)
* [Alternatives](#alternatives)
* [About](#about)
* [License](#license)

## Project Name

<table width="75%">
	<tr>
		<th>❗</th>
		<th align="left">Every project, no matter how trivial, should include this section.</th>
	</tr>
</table>

Choosing a project name can actually be quite difficult. Here are a few considerations to make.

### Including the language in the name

This can be a good idea if you plan to have multiple implementations of your project using different languages or if there is already an existing project or common name which you are implementing in another language.

* [CPython](https://github.com/python/cpython)
* [SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON)

### Googleability

Avoid using a generic word or a common combination of words for your project.
Selecting a somewhat unique name will make it easier for someone to search for your project.

## Shields

Shields are a great way to display important information about your project in a small amount of space.
Most shields you see on GitHub are from [Shields IO](http://shields.io/).
Shields are commonly displayed directly under the project name heading, sometimes above it.

![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg?style=flat)

A continuous integration status shield displays the build health of the project from a CI system like [Travis CI](https://travis-ci.org/).
The CI system will usually offer you a link you can copy-paste in your favorite format (HTML, Markdown, AsciiDoc, etc...).
The color of the shield will correspond to the build health.
Green means good, red means failure.

!["Build Status"](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)

By putting the license in a shield you make it easy for visitors to quickly determine if this project is compatible with theirs.
This shield should link to the license itself, either the official website or your embedded LICENSE file.
It's also common to link to [Software Licenses in Plain English](https://tldrlegal.com/).

!["Build Status"](https://img.shields.io/badge/release-v1.0.0-blue.svg?style=flat)

Let readers know the latest stable release by including this badge.
If the project is still young and hasn't had a stable release yet, it's common to make the badge orange or red to indicate that.

## Logo/Icon/Banner

<table width="75%">
	<tr>
		<th>💡</th>
		<th align="left">Use a tasteful size for your graphic, don't make it so large that you have to scroll far to get to useful information.</th>
	</tr>
</table>

<table width="75%">
	<tr>
		<th>💡</th>
		<th align="left">Remember to include alt-text on your images for accessibiliy.</th>
	</tr>
</table>

A graphic is commonly placed in one of the following locations:

* Above the project name header
	* Example: [Actor Messaging platform](https://github.com/actorapp/actor-platform/blob/d50649cdbddf3408ce4938b2c8e9861c0ed53249/README.MD)
	* Example: [osquery](https://github.com/facebook/osquery/blob/de8ef7b6274dc590cefa30eb997029754a911705/README.md)
* Right of the project name header and description
	* Example: [Awesome README](https://github.com/matiassingers/awesome-readme/blob/b143fc05d21d93e5e1c48db437092d9640ff0c52/readme.md)
	* Example: [bluebird](https://github.com/petkaantonov/bluebird/blob/4ce0226093fd0afa21a22518f9401d12ef38856b/README.md)
* Left of the short description
	* Example: [D3](https://github.com/d3/d3/blob/0806b7821fecc6a5af0e6ba4b52bbe49bf4e355f/README.md)
* In-line with the project name
	* Example: [RxSwift](https://github.com/ReactiveX/RxSwift/blob/208a84db0fb7c02f72d81e0ffcf5f511a5de8e82/README.md)
	* Example: [BitBar](https://github.com/matryer/bitbar/blob/9560dd45825bfddd9192a087069dc28434b43e94/README.md)
	* Example: [FlatBuffers](https://github.com/google/flatbuffers/blob/f624065eaa0c05f65dc0fcd4439ccda10cbef592/readme.md)
* Banner above the header 
	* Example: [Eureka](https://github.com/xmartlabs/Eureka/blob/f1a3ab894adc63b27b532d90f33bfe9088bc8518/README.md)
	* Example: [Carthage](https://github.com/Carthage/Carthage/blob/8e520a69556082afec8a7c45345c2de9a5d87df4/README.md)

## Download Badge

If your project is available for distribution through an app store or package manager they often provide badge assets to visually call out that your project is included.

!["Download on the App Store (Apple)"](https://camo.githubusercontent.com/0a78ccbf1b05e5b4ca4b14d9e7757aca1b0556ae/687474703a2f2f636c2e6c792f576f75472f446f776e6c6f61645f6f6e5f7468655f4170705f53746f72655f42616467655f55532d554b5f3133357834302e737667)

See [App Store Download Badge](https://developer.apple.com/app-store/marketing/guidelines/#downloadOnAppstore) for details on its use.

<img src="https://play.google.com/intl/en_us/badges/images/badge_new.png" alt="Google Play Download Badge" width=135>

See [Google Play Badge Page](https://play.google.com/intl/en_us/badges/) for details on its use.

## Short Description

<table width="75%">
	<tr>
		<th>❗</th>
		<th align="left">Every project, no matter how trivial, should include this.</th>
	</tr>
</table>

<table width="75%">
	<tr>
		<th>💡</th>
		<th align="left">If you are using GitHub then you should set the project description. The description is meta-data that appears in search results. You can re-use your opening sentence for this.</th>
	</tr>
</table>

Describe the most relevant high-level information in one short paragraph.
Try to get the most important information in the first two sentences.
The goal is to save the reader time by explaining the project's purpose.

Example Opening Sentences

* [Alamofire](https://github.com/Alamofire/Alamofire/blob/master/README.md)

	> Alamofire is an HTTP networking library written in Swift. 

* [Apache HTTP Server](http://svn.apache.org/repos/asf/httpd/httpd/trunk/README)

	> The Apache HTTP Server is a powerful and flexible HTTP/1.1 compliant web server.

* [D3.js](https://github.com/d3/d3/blob/master/README.md)

	> D3 (or D3.js) is a JavaScript library for visualizing data using web standards.

* [libgit2 README](https://github.com/libgit2/libgit2/blob/master/README.md)

	> libgit2 is a portable, pure C implementation of the Git core methods provided as a re-entrant linkable library with a solid API, allowing you to write native speed custom Git applications in any language with bindings.

## Table Of Contents Section

<table width="75%">
	<tr>
		<th>💡</th>
		<th align="left">This is optional, but if your README is long, you should include a TOC.</th>
	</tr>
</table>

Sometimes called "Contents".
If your README is long enough you might consider including a table of contents.
[AsciiDoc](http://asciidoc.org/) and [reStructuredText](http://docutils.sourceforge.net/rst.html) formats support automatic generation of the table of contents.

* Example: [Eureka](https://github.com/xmartlabs/Eureka/blob/f1a3ab894adc63b27b532d90f33bfe9088bc8518/README.md#contents)

## Screen Shots

If you include screenshots, set the width or height property to ensure they are not oversized.
This is especially important when your screenshots are from a high-dpi device but the README is being read on a low dpi-device.

## Feature List

Typically called just "Features".
A feature list can be a set of bullet points.
If you want to include commentary on each feature you can use sections instead.
If your feature list is very long or includes a lot of detail, consider putting it in its own file in the [Docs Directory](../How%20to%20Open%20Source.md#docs-directory) and linking to it from this section.

* Example: [Git Book](https://github.com/GitbookIO/gitbook/blob/f70da1c82a9a92c20a4771a1b321787a98a161c6/README.md#features)
* Example: [SQLite.swift](https://github.com/stephencelis/SQLite.swift/blob/f52bdc2fa499636d090d29aa4f88c5f5b0498399/README.md#features)

## Requirements

List the requirements for your project.
If you require a specific version of something, be sure to include that information.

* Example: [Swift](https://github.com/apple/swift/blob/e77f4ed8d9ec3428f4f4c7ce7df3ee09bd4bf921/README.md#system-requirements)
* Example: [Dokku](https://github.com/dokku/dokku/blob/a00a9219dae3921c22538f89751b8ae50b45e930/README.md#requirements)

## Installation

Ideally you will distribute your package as part of the appropriate repository.
For example, if this is a Perl project you might use CPAN, a Go library, use Go's manager, Node use npm etc...

* Example: [SwiftLint](https://github.com/realm/SwiftLint/blob/07313c09a52edfb9c9dbbbb87292317e2cef409e/README.md#installation)
* Example: [SQLite.swift](https://github.com/stephencelis/SQLite.swift/blob/f52bdc2fa499636d090d29aa4f88c5f5b0498399/README.md#installation)
* Example: [Dokku](https://github.com/dokku/dokku/blob/a00a9219dae3921c22538f89751b8ae50b45e930/README.md#installing)

## Configuration

⛔️ *ToDo: This section is a stub*

If your project is highly configurable consider making this its own document in the <<Docs Directory>> and linking to it from this section.

* Example: [SwiftLint](https://github.com/realm/SwiftLint/blob/07313c09a52edfb9c9dbbbb87292317e2cef409e/README.md#configuration)

## Usage/Quick Start

⛔️ *ToDo: This section is a stub*

Sometimes called "Guide" or "Tutorial" or "Getting Started".

* Example: [SwiftLint](https://github.com/realm/SwiftLint/blob/07313c09a52edfb9c9dbbbb87292317e2cef409e/README.md#usage)
* Example: [SQLite.swift](https://github.com/stephencelis/SQLite.swift/blob/f52bdc2fa499636d090d29aa4f88c5f5b0498399/README.md#usage)
* Example: [Git Book](https://github.com/GitbookIO/gitbook/blob/f70da1c82a9a92c20a4771a1b321787a98a161c6/README.md#usage-examples)
* Example: [Swift](https://github.com/apple/swift/blob/e77f4ed8d9ec3428f4f4c7ce7df3ee09bd4bf921/README.md#getting-started)
* Example: [Electron](https://github.com/electron/electron/blob/91ed01df26b6259ec55d84a8e3e44490ad4e21d0/README.md#quick-start)

## Documentation

If you hope to get people to use your project you will need to take documentation seriously. Some projects are small enough that they can fit all their documentation in the README itself ([example](https://github.com/xmartlabs/Eureka/blob/f1a3ab894adc63b27b532d90f33bfe9088bc8518/README.md#usage)). If it gets too long, then move it to the [Docs Directory](../How%20to%20Open%20Source.md#docs-directory) and refer to it from this section.

* Example: [traefik](https://github.com/containous/traefik/blob/5afcf1770690e29ae37de0ae53dbc20e808ba02a/README.md#documentation)
* Example: [Swift](https://github.com/apple/swift/blob/e77f4ed8d9ec3428f4f4c7ce7df3ee09bd4bf921/README.md#documentation)
* Example: [Electron](https://github.com/electron/electron/blob/91ed01df26b6259ec55d84a8e3e44490ad4e21d0/README.md#documentation)
* Example: [Eureka](https://github.com/xmartlabs/Eureka/blob/f1a3ab894adc63b27b532d90f33bfe9088bc8518/README.md#usage)
* Example: [Dokku](https://github.com/dokku/dokku/blob/a00a9219dae3921c22538f89751b8ae50b45e930/README.md#documentation)

## Examples

⛔️ *ToDo: This section is a stub*

## FAQ

⛔️ *ToDo: This section is a stub*

* Example: [Eureka](https://github.com/xmartlabs/Eureka/blob/f1a3ab894adc63b27b532d90f33bfe9088bc8518/README.md#faq)

## Troubleshooting

⛔️ *ToDo: This section is a stub*

This section is often included in projects whose documentation fits within the README. 

* Example: [Homebrew](https://github.com/Homebrew/brew/blob/33a8c993dd72c437efa972a85db5e6821b7a6107/README.md#troubleshooting)

## Non-Goals

This section is fairly uncommon, though it should be used more.
It can be very helpful to list things your project *isn't* meant for.
This can help limit the scope of your project and set expectations.
Non-goals can also help keep outside contributions and questions more focused on the project goals.

## Changes

Sometimes called "Version History".
Typically you would refer to and link the [CHANGELOG](../How%20to%20Open%20Source.md#changelog) file or releases section of your project site.

## Contributing

Typically this section just refers you to the [CONTRIBUTING](../How%20to%20Open%20Source.md#contributing) file. Even if it's already mentioned in the CONTRIBUTING file, it might be a good idea to state whether contributions are welcome.

* Example: [Swift](https://github.com/apple/swift/blob/e77f4ed8d9ec3428f4f4c7ce7df3ee09bd4bf921/README.md#contributing-to-swift)
* Example: [List of Free Learning Resources](https://github.com/vhf/free-programming-books/blob/ed903d3da0d867169fd9e55f93ea36e544383ac8/README.md#how-to-contribute)
* Example: [Xi Editor](https://github.com/google/xi-editor/blob/eeefa97550c0d9414fdb673114963f043844eb56/README.md#contributions)

## Contributors/Credits

May be called "Maintainers".
List of people who contributed to the project.
Yes, sites like GitHub already have a feature that let you see a list of contributors, and you can probably figure it out through the repo history too, but it might still be valuable to have this in the README because it lets you curate the list, order it based on influence or number of contributions, or take out old contributors who are no longer involved.

* Example: [Homebrew - Who Are You?](https://github.com/Homebrew/brew/blob/33a8c993dd72c437efa972a85db5e6821b7a6107/README.md#who-are-you)
* Example: [traefik - Maintainers](https://github.com/containous/traefik/blob/5afcf1770690e29ae37de0ae53dbc20e808ba02a/README.md#maintainers)
* Example: [traefik - Credits](https://github.com/containous/traefik/blob/5afcf1770690e29ae37de0ae53dbc20e808ba02a/README.md#credits)

## Security Disclosure

⛔️ *ToDo: This section is a stub*

* Example: [Docker](https://github.com/docker/docker/blob/68bf45084e3af9fa20d096b0d557bc1451aa5443/README.md#security-disclosure)
* Example: [bugcrowd/disclosure-policy](https://github.com/bugcrowd/disclosure-policy/blob/master/responsible_disclosure_policy.md)
* Example: [Homebrew](https://github.com/Homebrew/brew/blob/33a8c993dd72c437efa972a85db5e6821b7a6107/README.md#security)

## Donations

⛔️ *ToDo: This section is a stub*

* Example ([Bountysource](https://www.bountysource.com)): [XVim](https://github.com/XVimProject/XVim/blob/3eb09a6ffa68b4bc23b6d0703caea9e6152cd125/README.md#donations)
* Example (PayPal): [AdminLTE](https://github.com/almasaeed2010/AdminLTE/blob/2de98d7b70a130b350a30a5dda3ec4481e2437b6/README.md#donations)
* Example: [MacDown - Tipping](https://github.com/MacDownApp/macdown/blob/7cece8d2d9225658a4a2a65fd2f95780db377d67/README.md#tipping)
* Resource: [Create a PayPal Payment Button](https://www.paypal.com/buttons/paymentbuttons/donate/create)
* Example: [Homebrew](https://github.com/Homebrew/brew/blob/33a8c993dd72c437efa972a85db5e6821b7a6107/README.md#donations)

## Author(s)

Different from the [Contributors](#contributors) section in that this lists the original author(s) of the project. You may want to also include links to your blog and Twitter handle.

* Example: [Eureka](https://github.com/xmartlabs/Eureka/blob/f1a3ab894adc63b27b532d90f33bfe9088bc8518/README.md#authors)
* Example: [SQLite.swift](https://github.com/stephencelis/SQLite.swift/blob/f52bdc2fa499636d090d29aa4f88c5f5b0498399/README.md#author)
* Example: [Xi Editor](https://github.com/google/xi-editor/blob/eeefa97550c0d9414fdb673114963f043844eb56/README.md#authors)

## Support/Help

⛔️ *ToDo: This section is a stub*

See next section: [Community/Communication](#communitycommunication).

* Example: [Git Book](https://github.com/GitbookIO/gitbook/blob/f70da1c82a9a92c20a4771a1b321787a98a161c6/README.md#help-and-support)

## Community/Communication

Depending on what type of community groups exist for your project, you might point users to: stackoverflow, irc, mailing lists, slack, wiki, forums etc...

* Example: [Electron](https://github.com/electron/electron/blob/91ed01df26b6259ec55d84a8e3e44490ad4e21d0/README.md#community)
* Example: [MacDown - Discussion](https://github.com/MacDownApp/macdown/blob/7cece8d2d9225658a4a2a65fd2f95780db377d67/README.md#discussion)
* Example: [SQLite.swift](https://github.com/stephencelis/SQLite.swift/blob/f52bdc2fa499636d090d29aa4f88c5f5b0498399/README.md#communication)

## Commercial Support

Often commercial support is simply mentioned in a sentence in the [Community/Communication](#communitycommunication) section, referring to the maintainer's email for details on commercial support.

* Example: [Java Native Access (JNA)](https://github.com/java-native-access/jna/blob/bbc36004c347c41858ac32a2ce7f9752a2f11ae1/README.md#community-and-support)
* Example: [traefik](https://github.com/containous/traefik/blob/5afcf1770690e29ae37de0ae53dbc20e808ba02a/README.md#support)

## Sponsors

Sufficiently large projects may receive funding and list their sponsors here. You can also provide details about how to become a sponsor. Sometimes this is name "Backers".

* Example: [Dokku](https://github.com/dokku/dokku/blob/a00a9219dae3921c22538f89751b8ae50b45e930/README.md#sponsors)
* Example: [Homebrew](https://github.com/Homebrew/brew/blob/33a8c993dd72c437efa972a85db5e6821b7a6107/README.md#sponsors)

## Projects Using X

If your project is being used by other projects or well known entities you can list them here.

* Example: [Java Native Access (JNA)](https://github.com/java-native-access/jna/blob/bbc36004c347c41858ac32a2ce7f9752a2f11ae1/README.md#projects-using-jna)

## Disclaimer

Most software licenses will typically include a disclaimer so this section isn't necessary most of the time.
If people might jump to certain conclusions about your project it might be a good idea to call it out in its own section.
Another reason to add a disclaimer would be to distance your project from your employer, if it might be easy to draw conclusions about their involvement.

* Example: [Malcom - Malware Communication Analyzer](https://github.com/tomchop/malcom/blob/master/README.md)
* Example: [Investing Returns on the S&P500](https://github.com/zonination/investing/blob/master/README.md)
* Example: [Xi Editor](https://github.com/google/xi-editor/blob/eeefa97550c0d9414fdb673114963f043844eb56/README.md#disclaimer)

## Related Projects

If your project may have plug-ins or extensions it may be a good idea to list some of them here.

* Example: [SQLite.swift](https://github.com/stephencelis/SQLite.swift/blob/f52bdc2fa499636d090d29aa4f88c5f5b0498399/README.md#related)

## Alternatives

Projects rarely include this section, but it could be helpful to the reader.
You don't have to exhaustively list every similar library, but mentioning a few common ones can be useful.

* Example: [SQLite.swift](https://github.com/stephencelis/SQLite.swift/blob/f52bdc2fa499636d090d29aa4f88c5f5b0498399/README.md#alternatives)

## About

⛔️ *ToDo: This section is a stub*

* Example: [SwiftLint](https://github.com/realm/SwiftLint/blob/07313c09a52edfb9c9dbbbb87292317e2cef409e/README.md#about)

## License

<table width="75%">
	<tr>
		<th>❗</th>
		<th align="left">You should always include a license with your project.</th>
	</tr>
</table>

Although you probably already have a [shield](#shields) with the license, it doesn't hurt to explicitly call it out again here.
This is typically the last section of the README.
If the license is short you can include the contents, otherwise link to the LICENSE file.
Even if it's obvious it does help to actually mention the name of the license instead of just including its contents.
For example: say it's "MIT", "2-clause BSD" etc...

* Example: [SwiftLint](https://github.com/realm/SwiftLint/blob/07313c09a52edfb9c9dbbbb87292317e2cef409e/README.md#license)

Many projects now use [FOSSA](https://fossa.io/) to track license compliance and attribution.

* Example: [NervJS license section](https://github.com/NervJS/nerv#license)
