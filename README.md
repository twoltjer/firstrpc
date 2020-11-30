# First RP Site Development

## Initial set up

1. Install `RubyGems` and `bash` using a downloaded executable or your package manager. `bash` is available on most non-Windows systems by default. 

2. Install required gems packages. Ensure that the binary install directory (`~/.gem/ruby/2.7.0/bin` on my system) is incldued your `PATH` variable. If it is not, the install command will display a warning. 

```shell script
$ gem install bundler jekyll jekyll-feed jekyll-seo-tag
```

3. Clone the git repository which contains the source code for the site. 

```shell script
$ git clone git@github.com:twtduck/firstrpc.git
```

The folder downloaded to `firstrpc` contains the development files for the site. 

## Structure and Development

The site is built on jekyll, using a variation of the minima theme. 

### Structure

`_includes` contains HTML snippets for code resused throughout the site.

`_layouts` contains layout templates. Generally, only use the `page` template.

`_plugins` defines plugins that are used in the site. 

Media files (such as images) for the site are organized in the `Media` directory.

### Plugins

Currently, only the `kramdown` plugin is used. This allows pages in the site to use both HTML and markdown in the same file. For instance, a centered welcome banner could be added:

```markdown
<div class="centered">
{% markdown %}

![Welcome](/Media/Welcome_Banner.png)

{% endmarkdown %}
</div>
```



### 
