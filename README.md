# Leonids Theme for Hugo

Leonids is a port of a [Jekyll Theme](https://github.com/renyuanz/leonids) to Hugo.

## Leonids is :
  * Responsive templates. Trying to look good on mobile, tablet and desktop.
  * Javascript Free.
  * Built with TableofContent support.
  * Built with Pure CSS Lightbox and a shortcode added to simplify the writing.
  * Trying to be simple and extensible.
  * **And** the Leonids (/ˈliːənɪdz/ lee-ə-nidz) are a prolific meteor shower associated with the comet [Tempel-Tuttle](https://en.wikipedia.org/wiki/55P/Tempel%E2%80%93Tuttle).

## Lightbox Shortcode.

It all started with the choosing of [Pure CSS Lightbox](http://youmightnotneedjs.com/#lightbox) for the main lightbox of Leonids. I tends to prefer Javascriptless websites on the Web. I created a simple shortcode for Hugo to simplify the writing :
```
<p><a href="#{{ .Get "href" }}">
  <img src="{{ .Get "src" }}" class="thumbnail"   width="{{ .Get "width" }}" alt="{{ .Get "alt" }}">
</a>
<a href="#_" class="lightbox" id="{{ .Get "href" }}">
  <img src="{{ .Get "src" }}" alt="{{ .Get "alt" }}">
</a></p>
```
And it can be put on your markdown files with :
```
{{< lightbox href="#img1" src="" width="" alt="">}}
```

## TODO
- [ ] Static comments powered with YAML/Mail.
