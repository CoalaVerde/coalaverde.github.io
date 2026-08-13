# coalaverde.github.io

<style>
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
}

.spinning-circle {
  position: relative;
  display: flex;
  border-radius: 50%;
  float: left;
  shape-outside: circle(50%);
  shape-margin: 0.5em;
  box-shadow: 0px 0px 10px 15px rgba(0,0,0,0.5);
}

/* The spinning dashed border layer */
.spinning-circle::before {
  content: '';
  position: absolute;
  inset: -4px; /* Expands the border outward */
  border: 10px dashed #91bc1f;
  border-radius: 50%;
  animation: spin 30s linear infinite;
}

.spinning-circle::after {
  content: '';
  position: absolute;
  inset: 2px;
  border: 5px solid rgba(0,0,0,0.5);
  border-radius:50%;
  box-shadow: inset 0px 0px 10px 5px rgba(0,0,0,0.4);
}

.spinning-circle:hover::after {
  inset: -2px;
}

/* Rotation keyframes */
@keyframes spin {
  100% {
    transform: rotate(360deg);
  }
}

footer {
  max-width: 100%;
  color: #333333;
  text-shadow: 0px 1px 0px rgba(255, 255, 255, 0.3);
}
</style>
<p>
<a float="left" href="https://codeberg.org/Kurt.Cobain" target="_blank">
  <img src="https://img.shields.io/badge/Codeberg-Follow me-dodgerblue?style=social&logo=codeberg" alt="Codeberg - Kurt.Cobain"></a>
<a float="right" href="https://github.com/CoalaVerde"><img alt="GitHub followers" src="https://img.shields.io/github/followers/CoalaVerde"></a>
</p>
<div class="spinning-circle" style="margin-right: 1em; max-width:30%;">
<img alt="A kitten running from two creepers on a bright grass field" src="/avatar.png" style="outline-offset: -6px;outline:10px solid white;border-radius: 50%;">
</div>
Hi there, this is my website :-).

I like embedded/retro/experimental systems and ways to work around its limitations. I also like <a title="Like Plan9" href="https://en.wikipedia.org/wiki/Distributed_computing">distributed</a> and <a title="Like those old DECs in the 70s" href="https://en.wikipedia.org/wiki/Shell_account">shared computing</a>.

This is my first time using Jekyll and Github Pages, thus this is right now just a placeholder and I will improve it later.

I speak _English_ <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Flag-us.svg" width="20px"> <sup>(B1/B2)</sup> and _Spanish_ <img src="https://upload.wikimedia.org/wikipedia/commons/f/fe/Flag-es.svg" width="20px"> <sup>(Native)</sup>.

Mildly fluent at _Bash_ <img src="https://upload.wikimedia.org/wikipedia/commons/6/66/Utilities-terminal.svg" width="20px"> and learning _Python_ <img src="https://upload.wikimedia.org/wikipedia/commons/0/0a/Python.svg" width="20px">

## Projects
<ul>
<li><a href="https://github.com/CoalaVerde/Marble-Appimage" target="_blank">
  <img src="https://img.shields.io/badge/Marble%20Browser-Appimage-blue?style=plastic&link=https%3A%2F%2Fgithub.com%2FCoalaVerde%2FMarble-Appimage"></a>
</li>
<ul>
<li><strong>Continuous Github Actions:</strong> Scheduled Appimage builds for the Marble browser upon new release from upstream.</li></ul>
</ul>
<img alt="Coming Soon" src="https://img.shields.io/badge/Coming-Soon-purple?style=for-the-badge&logo=Skeleton">

### Send me a push notification!
<div class="ntfy-box">
  <textarea rows="3" cols="30" style="margin-bottom: 10px" id="ntfy-input" placeholder="Type a message"></textarea>
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
