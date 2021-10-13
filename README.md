## Texas Advanced Computing Center
# Django CMS Plugin: "Callout"

This plugin render a "callout" a.k.a. "call to action".

- __`__plugin_name__`__: `taccsite_callout`
- __`__PluginName__`__: `TaccsiteCallout`
- __"Plugin Name"__: "Callout"

## Quick Start

1. Follow https://github.com/tacc-wbomar/Core-CMS-Plugin/wiki/Core-CMS-Plugin-Usage-Quick-Start.

## Usage

1. Add instance of plugin to a page.
1. Configure the plugin instance.
1. (Optional) Add and nest plugin instances to support extra content.
1. See plugin render content that matches configuration (and nested plugin instances).

[dcms-picture]: https://github.com/django-cms/djangocms-picture

## Features

1. Renders title and descritpion in a highlighted block.
1. Renders supported, nested plugin instances to incorporate extra content.
    <details>

    | content | supported by |
    | :- | :- |
    | image | [`djangocms-picture`][dcms-picture] |

    </details>

## Caveats

- The "Advanced settings" field "Resize any image to fit" causes image in page preview to disappear after saving the plugin.
    <details>

    _This is because of a JavaScript race condition. Using a server-side solution would eliminate this caveat. See [TACC/Core-CMS#327](https://github.com/TACC/Core-CMS/issues/327)._

    _The issue is called out in the admin form using user-oriented language._

    </details>
- Control over image cropping is not supported through the admin form.
    <details>

    _Cropping options could be implemented via CSS or a feature of https://github.com/django-cms/django-filer. For details, see [TACC/Core-CMS#329](https://github.com/TACC/Core-CMS/issues/329)._

    </details>
