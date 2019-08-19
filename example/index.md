<!-- njnmdoc:  title="njnmdoc"  -->

From: [Neal Fultz](https://njnm.co) &lt;[neal@njnm.co](mailto:neal@njnm.co)&gt;

<a href="https://github.com/njnmco/njnmdoc" class="github-corner" aria-label="View source on GitHub"><svg width="80" height="80" viewBox="0 0 250 250" style="fill:#70B7FD; color:#fff; position: absolute; top: 0; border: 0; right: 0;" aria-hidden="true"><path d="M0,0 L115,115 L130,115 L142,142 L250,250 L250,0 Z"></path><path d="M128.3,109.0 C113.8,99.7 119.0,89.6 119.0,89.6 C122.0,82.7 120.5,78.6 120.5,78.6 C119.2,72.0 123.4,76.3 123.4,76.3 C127.3,80.9 125.5,87.3 125.5,87.3 C122.9,97.6 130.6,101.9 134.4,103.2" fill="currentColor" style="transform-origin: 130px 106px;" class="octo-arm"></path><path d="M115.0,115.0 C114.9,115.1 118.7,116.5 119.8,115.4 L133.7,101.6 C136.9,99.2 139.9,98.4 142.2,98.6 C133.8,88.0 127.5,74.4 143.8,58.0 C148.5,53.4 154.0,51.2 159.7,51.0 C160.3,49.4 163.2,43.6 171.4,40.1 C171.4,40.1 176.1,42.5 178.8,56.2 C183.1,58.6 187.2,61.8 190.9,65.4 C194.5,69.0 197.7,73.2 200.1,77.6 C213.8,80.2 216.3,84.9 216.3,84.9 C212.7,93.1 206.9,96.0 205.4,96.6 C205.1,102.4 203.0,107.8 198.3,112.5 C181.9,128.9 168.3,122.5 157.7,114.1 C157.9,116.9 156.7,120.9 152.7,124.9 L141.0,136.5 C139.8,137.7 141.6,141.9 141.8,141.8 Z" fill="currentColor" class="octo-body"></path></svg></a><style>.github-corner:hover .octo-arm{animation:octocat-wave 560ms ease-in-out}@keyframes octocat-wave{0%,100%{transform:rotate(0)}20%,60%{transform:rotate(-25deg)}40%,80%{transform:rotate(10deg)}}@media (max-width:500px){.github-corner:hover .octo-arm{animation:none}.github-corner .octo-arm{animation:octocat-wave 560ms ease-in-out}}</style>

njnmdoc is a light text-based static site generator descending from [jemdoc][].
Although the majority of the code has changed, the core ideas remain the same.
It takes a text file written with [markdown][], an optional configuration file
and an optional menu file, and makes websites that look something like this
one.

> Version *8.1.0* was released on 2019-06-05.
> See the [release notes](revision.html).

[Download njnmdoc][download] or [contribute on Github][github]

## Goals

  - Simple, consistent syntax via Markdown (multiple backends).
  - \\(\LaTeX\\) equation support via [KaTex][katex].
  - Portability. The (single) `njnmdoc` [Python][] script +
    single css stylesheet + your input file &rarr; html.
  - Based on [CSS][] so formatting and layout specifics are
    independent of content.
  - Produces clean, [standards-compliant][validator] [XML 1.1][xml].
  - Minimal bells and whistles.

## Configuration

### Modelines

<h2 id="markdown">Markdown</h2>

`njnmdoc` supports the following markdown processors:

  - `markdown` python package
  - `markdown` perl script
  - `pandoc`
  - GitHub Markdown API

<h2 id="math-mode">Math Mode</h2>

<h2 id="menus">Menus</h2>

A menu can be included into each document by specifying the appropriate option in the modeline or the config file. It will be parsed as markdown.


## License
Copyright (&copy;)
2007-2012 Jacob Mattingley,
2012-2015 Wonseok Shin,
2019 Neal Fultz

njnmdoc is free software; you can redistribute it and/or modify it under the
terms of the [GNU General Public License][gpl] as published by the Free
Software Foundation; either version 3 of the License, or (at your option) any
later version.

njnmdoc is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the [GNU General Public License][gpl] for more details.


[markdown]: https://daringfireball.net/projects/markdown/
[gpl]: http://www.gnu.org/licenses/gpl-3.0.html
[python]: http://www.python.org
[css]: http://www.w3.org/Style/CSS/
[xml]: http://www.w3.org/TR/xhtml11/
[validator]: http://validator.w3.org/check/referer
[download]: https://github.com/njnmco/njnmdoc/raw/master/njnmdoc
[github]: http://github.com/njnmco/njnmdoc
[katex]: https://katex.org
[jemdoc]: https://jemdoc.jaboc.net
