# project: Sekai Kernel <br>

#### Roadmap:
- [x] Boot Sekai kernel for first time
- [x] Make client code Posix Standard and Windows NT compatiable
- [x] Create Custom Networking protocol
- [ ] Create Sekai messanging system (ITCP Inter Thread Communication Protocol API)
- [ ] Create Hot Reloadable Threads API 
- [ ] Create Render  

#### Release (approx) in: 
```html
<p id="time-text" style="color: #daa520;"> <span id="time">28d 20h 48m 14s </span> </p>

<script>
	var countDownDate = new Date("Aug 26, 2026 00:00:00").getTime();
	var x = setInterval(function() {
 	var now = new Date().getTime();
	var distance = countDownDate - now;

  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  document.getElementById("time").innerHTML = days + "d " + hours + "h " + minutes + "m " + seconds + "s ";

  if (distance < 0) {
    clearInterval(x);
    document.getElementById("time").innerHTML = "Beta avaible for test now!";
    document.getElementById("time-text").innerHTML = "";
  }
}, 1000);
</script>
```

