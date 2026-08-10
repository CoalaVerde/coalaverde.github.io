# coalaverde.github.io

<style>
a {
  display:inline flow-root;
}
a.dfn-hover {
	color: #333;
	text-decoration: none;
}
dfn {
  border-bottom: dashed 1px rgba(0,0,0,0.8);
  padding: 0 0.4em;
  font-style: normal;
  position: relative;
}
dfn::after {
  content: attr(data-info);
  display: inline;
  position: absolute;
  top: 22px; left: 0;
  opacity: 0;
  width: 230px;
  font-size: 13px;
  font-weight: 700;
  line-height: 1.5em;
  padding: 0.5em 0.8em;
  background: rgba(0,0,0,0.8);
  color: #fff;
  pointer-events: none; /* This prevents the box from apearing when hovered. */
  transition: opacity 250ms, top 250ms;
	white-space: pre-wrap;
}
dfn::before {
/*  content: '';
  display: block;
  position: absolute;
  top: 12px; left: 20px;
  opacity: 0;
  width: 0; height: 0;
  border: solid transparent 5px;
  border-bottom-color: rgba(0,0,0,0.8);
  transition: opacity 250ms, top 250ms;
}*/
dfn:hover {z-index: 2;} /* Keeps the info boxes on top of other elements */
dfn:hover::after,
dfn:hover::before {opacity: 1;}
dfn:hover::after {top: 30px;}
dfn:hover::before {top: 20px;}
</style>
<p>
<a float="left" href="https://codeberg.org/Kurt.Cobain" target="_blank">
  <img src="https://img.shields.io/badge/Codeberg-Follow me-dodgerblue?style=social&logo=codeberg" alt="Codeberg - Kurt.Cobain"></a>
<a float="right" href="https://github.com/CoalaVerde"><img alt="GitHub followers" src="https://img.shields.io/github/followers/CoalaVerde"></a>
</p>
<img alt="A kitten running from two creepers on a bright grass field" src="/tinyavatar.jpg" style="shape-outside: circle(); shape-margin: 1em; margin-right: 1em ; float: left; border-radius: 50%; max-width: 50%; outline: dotted white 1px;">
Hi there, this is my website :-).

I like embedded/retro/experimental systems and ways to work around its limitations. I also like <dfn data-info="See for example Plan 9 from Bell Labs"><a href="https://en.wikipedia.org/wiki/Distributed_computing">distributed</a></dfn> and <dfn data-info="See for example the SDF pubnix and tildeverse.org"><a href="https://en.wikipedia.org/wiki/Shell_account">shared computing</a></dfn>.

This is my first time using Jekyll and Github Pages, thus this is right now just a placeholder and I will improve it later.

I speak _English_ <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Flag-us.svg" width="2%"> <sup>(B1/B2)</sup> and _Spanish_ <img src="https://upload.wikimedia.org/wikipedia/commons/f/fe/Flag-es.svg" width="2%"> <sup>(Native)</sup>. Mildly fluent at _Bash_ <img src="https://upload.wikimedia.org/wikipedia/commons/6/66/Utilities-terminal.svg" width="2%"> and learning _Python_ <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Python.svg" width="2%">

## Projects
<li><a href="https://github.com/CoalaVerde/Marble-Appimage" target="_blank">
  <img src="https://img.shields.io/badge/Marble%20Browser-Appimage-blue?style=plastic&link=https%3A%2F%2Fgithub.com%2FCoalaVerde%2FMarble-Appimage"></a>
</li>
<ul><strong>Continuous Github Actions:</strong> Scheduled Appimage builds for the Marble browser upon new release from upstream.</ul>
<img alt="Coming Soon" src="https://img.shields.io/badge/Coming-Soon-purple?style=for-the-badge&logo=Skeleton">
<hr>
<p style="display: inline flow-root; float: left;">Copywrong • 2026</p>
<p style="display: inline flow-root; float: right; text-align: right;"><a href="https://github.com/CoalaVerde/coalaverde.github.io"><img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/CoalaVerde/coalaverde.github.io?logo=github"></a></p>
