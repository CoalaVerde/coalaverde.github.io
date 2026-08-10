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
  /*content: '';*/
  display: block;
  position: absolute;
  top: 12px; left: 20px;
  opacity: 0;
  width: 0; height: 0;
  border: solid transparent 5px;
  border-bottom-color: rgba(0,0,0,0.8);
  transition: opacity 250ms, top 250ms;
}
dfn:hover {z-index: 2;} /* Keeps the info boxes on top of other elements */
dfn:hover::after,
dfn:hover::before {opacity: 1;}
dfn:hover::after {top: 30px;}
dfn:hover::before {top: 20px;}

button {
	color:white;
  	border:1px solid #5d910b;
  	background:linear-gradient(#93bd20, #659e10);
  	border-radius:2px;
  	box-shadow:inset 0px 1px 0px rgba(255,255,255,0.3),0px 3px 7px rgba(0,0,0,0.7);
  	background-color:#93bd20;
  	padding:10px 12px;
  	margin-top:6px;
  	line-height:14px;
  	font-size:14px;
  	display:inline-block;
	text-align:center
}
button:hover {
  background:linear-gradient(#749619, #527f0e);
  background-color:#659e10;
  border:1px solid #527f0e;
  box-shadow:inset 0px 1px 1px rgba(0,0,0,0.2),0px 1px 0px transparent
}
textarea {
  color: #fff;
  padding:8px 15px;
  background:#191919;
  border-radius:2px;
  border:1px solid #121212;
  box-shadow:inset 0 1px 3px rgba(0,0,0,0.3);
  overflow:auto;
  overflow-y:hidden

.spinning-circle {
  position: relative;
  width: 120px;
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #222;
  color: #fff;
  border-radius: 50%;
}

/* The spinning dashed border layer */
.spinning-circle::before {
  content: '';
  position: absolute;
  inset: -8px; /* Expands the border outward */
  border: 4px dashed #fff;
  border-radius: 50%;
  animation: spin 8s linear infinite;
}

/* Rotation keyframes */
@keyframes spin {
  100% {
    transform: rotate(360deg);
  }
}

}
</style>
<p>
<a float="left" href="https://codeberg.org/Kurt.Cobain" target="_blank">
  <img src="https://img.shields.io/badge/Codeberg-Follow me-dodgerblue?style=social&logo=codeberg" alt="Codeberg - Kurt.Cobain"></a>
<a float="right" href="https://github.com/CoalaVerde"><img alt="GitHub followers" src="https://img.shields.io/github/followers/CoalaVerde"></a>
</p>
<img alt="A kitten running from two creepers on a bright grass field" src="/avatar.png" class="spinning-circle" style="shape-outside: circle(); shape-margin: 1em; margin-right: 1em ; float: left; border-radius: 50%; max-width: 45%; outline: dashed white 2px; padding: 2px">
Hi there, this is my website :-).

I like embedded/retro/experimental systems and ways to work around its limitations. I also like <dfn data-info="See for example Plan 9 from Bell Labs"><a href="https://en.wikipedia.org/wiki/Distributed_computing">distributed</a></dfn> and <dfn data-info="See for example the SDF pubnix and tildeverse.org"><a href="https://en.wikipedia.org/wiki/Shell_account">shared computing</a></dfn>.

This is my first time using Jekyll and Github Pages, thus this is right now just a placeholder and I will improve it later.

I speak _English_ <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Flag-us.svg" width="20px"> <sup>(B1/B2)</sup> and _Spanish_ <img src="https://upload.wikimedia.org/wikipedia/commons/f/fe/Flag-es.svg" width="20px"> <sup>(Native)</sup>. Mildly fluent at _Bash_ <img src="https://upload.wikimedia.org/wikipedia/commons/6/66/Utilities-terminal.svg" width="20px"> and learning _Python_ <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Python.svg" width="20px">

## Projects
<li><a href="https://github.com/CoalaVerde/Marble-Appimage" target="_blank">
  <img src="https://img.shields.io/badge/Marble%20Browser-Appimage-blue?style=plastic&link=https%3A%2F%2Fgithub.com%2FCoalaVerde%2FMarble-Appimage"></a>
</li>
<ul><strong>Continuous Github Actions:</strong> Scheduled Appimage builds for the Marble browser upon new release from upstream.</ul>
<img alt="Coming Soon" src="https://img.shields.io/badge/Coming-Soon-purple?style=for-the-badge&logo=Skeleton">

### Send me a push notification!
<div class="ntfy-box">
  <textarea rows="3" cols="50" style="margin-bottom: 10px" id="ntfy-input" placeholder="Type a message"></textarea>
  <button onclick="javascript:sendNotification()" style="margin-left:10px; margin-bottom: 10px">Send</button>
</div>

<script>
  // stolen ntfy script
  function send(message) {
    let r = new XMLHttpRequest()
    r.open("POST", "https://ntfy.sh/coalaverdegithubio", true)
    r.setRequestHeader("Content-Type", "text/plain")
    r.send(message)
  }
  // send notification
  let ntfyInput = document.getElementById("ntfy-input")
  function sendNotification() {
    if (ntfyInput.value.length <= 0) return
    send(ntfyInput.value)
    ntfyInput.value = ""
  }
</script>
<hr>
<footer>
<p style="display: inline flow-root; float: left;">Copywrong • 2026</p>
<p style="display: inline flow-root; float: right; text-align: right;"><a href="https://github.com/CoalaVerde/coalaverde.github.io"><img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/CoalaVerde/coalaverde.github.io?logo=github"></a></p>
</footer>
