# Showcase Template

Welcome to the [gohugo](https://gohugo.io/) template to create rich content [academic reports](https://www.wordy.com/writers-workshop/writing-an-academic-report/) having [p5.js](https://p5js.org/) sketches.

## Hacking

Install the [gohugo](https://gohugo.io/) [static site generator](https://jamstack.org/generators/) then:

```sh
$git clone https://github.com/objetos/showcase
$cd showcase
$git submodule update --init --recursive
$hugo server -D --disableFastRender
```

Deploy with `$git push` after redefining `baseURL` in `config.toml` which should point to your actual public remote.

The template uses the [hugo-book](https://github.com/alex-shpak/hugo-book) theme by default. Check the [hugo themes site](https://themes.gohugo.io/) if you wish to add other ones.

Note that deployment is implemented with a [github action](https://github.com/features/actions) which parses the source code from the repo `main` branch into the `html` generated page found (and served) at the repo `gh-pages` branch. If you forked the repo don't forget to activate the repo workflow [actions](https://github.com/objetos/showcase/actions).

If you changed the repo name don't forget to update all the js related (both sketches and assets) urls.

If you are unfamiliar with [git](https://git-scm.com/) check out this [tutorial series](https://thecodingtrain.com/beginners/git-and-github/) and also this [presentation](https://objetos.github.io/git).