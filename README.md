# Clean White Gisma Theme for Hugo

CleanWhite is a clean, elegant, but fully functional blog theme for Hugo. [gi-modules](https://gisma-courses.github.io/gi-modules) provides a live demo

It is based on [huxblog Jekyll Theme](https://github.com/Huxpro/huxpro.github.io)
and [Clean Blog Jekyll Theme](https://github.com/BlackrockDigital/startbootstrap-clean-blog-jekyll).

These two upstream projects have done awesome jobs to create a blog theme, what I'm doing here is porting it to Hugo, of which I like the simplicity and the much faster compiling speed. Some other features which I think could be useful, such as site search with algolia and proxy for Disqus access in China, have also been built in the CleanWhite theme. Other fancy features of upstream projects are not supported by this Hugo theme, I'd like to make it as simple as possible and only focus on blog purpose, at least for now.
While I created this theme, I followed the Hugo theme best practice and tried to make every part of the template as a replaceable partial html, so it could be much easier for you to make your customization based on it.

## Quick Start

The simplest way is to start with the example site coming with this theme, then you can play around and add your own stuff.

```
$ mkdir test
$ cd test
$ mkdir themes
$ cd themes
$ git clone (https://github.com/gisma-courses/hugo-theme-cleanwhite-gisma.git
$ cp -r hugo-theme-cleanwhite-gisma/exampleSite/** ../
$ cd ..
$ hugo serve
```

If your site is already a git project, you may want to choose to add the cleanwhite theme as a submodule to avoid messing up your existing git repository.

```
$ mkdir themes
$ git submodule add https://github.com/gisma-courses/hugo-theme-cleanwhite-gisma.git themes/hugo-theme-cleanwhite-gisma
```
Run  Hugo Build-in Server Locally

```
$ hugo serve -t  hugo-theme-cleanwhite-gisma
```
Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser.

For more information read the official [setup guide](https://gohugo.io/overview/installing/) of Hugo

### Comments
The comments system is powered by [utterances](https://utteranc.es/) via github. 

### Analytics

You can optionally enable Google Analytics. Type your tracking code in the

```toml
googleAnalytics = "UA-XXXXX-X"
ba_track_id  = "XXXXXXXXXXXXXXXX"
```
Leave the `googleAnalytics`  or 'ba_track_id ' key empty to disable it.

### Mind Map

Mind Map is supported with shortcode 'mind', instering the following code snippet into  your markdown file can create a mind map showing in the screenshots.

```markdown
{{% mind %}}
- Root
    - Level 1
        - Level 2
        - Level 2
            - Level 3
            - Level 3
                - Level 4
                    - Level 5
                        - Level 6
    - Level 1
        - Level 2
        - Level 2
     - Level 1
        - Level 2
        - Level 2
     - Level 1
        - Level 2
        - Level 2
     - Level 1
        - Level 2
        - Level 2
{{% /mind %}}
```

### Embedded Videos

Use the below hugo shortcodes to embed videos into your posts.

Youtube
```
{{< youtube jgbTosOPU-U >}}
```

Vimeo
```
{{< vimeo 514140603 >}}
```

## Thanks
Thanks for the great jobs of [huxblog Jekyll Theme](https://github.com/Huxpro/huxpro.github.io) and [Clean Blog Jekyll Theme](https://github.com/BlackrockDigital/startbootstrap-clean-blog-jekyll) which are the the two upstream projects CleanWhite Hugo theme is based on. In addition the gisma Version is just a teak of the [hugo-theme-cleanwhite](https://github.com/zhaohuabing) of Zhao Huabing.

## Feedback
If you find any problems, please feel free to [raise an issue](https://gisma-courses.github.io/hugo-theme-cleanwhite-gisma/issues/new) or create a pull request to fix it.


