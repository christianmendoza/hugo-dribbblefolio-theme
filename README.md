# DribbleFolio

DribbbleFolio is a Dribbble-integrated One Page HTML portfolio template to showcase your latest Dribbble shots. It is a port of [DribbleFolio](//dribbble.com/shots/2035170-DribbbleFolio-Dribbble-Portfolio-HTML-Template-Free-Download) by [Vineeth Gopal](//dribbble.com/gsvineeth).

![Hugo DribbleFolio Theme screenshot](https://raw.githubusercontent.com/christianmendoza/hugo-dribbblefolio-theme/master/images/screenshot.png)


## Installation

Inside the folder of your Hugo site run:

    $ cd themes
    $ git clone https://github.com/christianmendoza/hugo-dribbblefolio-theme

For more information read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.


## Getting started

After installing the DribbleFolio theme successfully it requires a just a few more steps to get your site finally running.


### The config file

Take a look inside the [`exampleSite`](//github.com/christianmendoza/hugo-dribbblefolio-theme/tree/master/exampleSite) folder of this theme. You'll find a file called [`config.toml`](//github.com/christianmendoza/hugo-dribbblefolio-theme/blob/master/exampleSite/config.toml). To use it, copy the [`config.toml`](//github.com/christianmendoza/hugo-dribbblefolio-theme/blob/master/exampleSite/config.toml) in the root folder of your Hugo site. Feel free to customize this theme as you like.


### Configure Dribbble

You have two options to fetch and show your latest Dribbble shots: static or dynamic. Setting `static` to `true` will fetch your shots only every Hugo build using the [`getJSON`](//gohugo.io/templates/data-templates/#implementation-details) Hugo function. Updating with new shots will require a new Hugo build (and upload). If you want a more dynamic method, set `static` to `false`, which utilizes the jQuery plugin [jribbble](//github.com/tylergaw/jribbble).

Set your Dribbble client access token in `token`. If you don't have a token, create a new app and get it at [https://dribbble.com/account/applications/new](https://dribbble.com/account/applications/new)

Set your Dribbble username in `userId`.

`perPage` controls how many shots you want to fetch and show. The maximum you can set here is `100` per Dribbble's API.


```toml
[params.dribbble]
  static = true
  token = ""
  userId = ""
  perPage = 12
```


### Nearly finished

In order to see your site in action, run Hugo's built-in local server.

    $ hugo server

Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser.


## Contributing

Did you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](//github.com/christianmendoza/hugo-dribbblefolio-theme/issues) to let me know. Or make directly a [pull request](//github.com/christianmendoza/hugo-dribbblefolio-theme/pulls).


## License

The original template is released under the [Creative Commons Attribution 3.0 License](//github.com/christianmendoza/hugo-dribbblefolio-theme/blob/master/LICENSE.md).


## Annotations

- Original [DribbleFolio](//dribbble.com/shots/2035170-DribbbleFolio-Dribbble-Portfolio-HTML-Template-Free-Download) Template by [Vineeth Gopal](//dribbble.com/gsvineeth)

Also thanks to [Steve Francia](//github.com/spf13) for creating [Hugo](//gohugo.io) and the awesome community around the project.
