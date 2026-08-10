<!doctype html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width,initial-scale=1" />
	<title>Billie & Nicole — Wedding Invitation</title>
	<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700&family=Montserrat:wght@300;400;600&display=swap" rel="stylesheet">
	<link rel="stylesheet" href="https://unpkg.com/aos@2.3.1/dist/aos.css" />
	<style>
		:root{
			--cream:#f7efe6;
			--ivory:#fffaf1;
			--brown:#2e1f18;
			--mocha:#3b2a23;
			--gold:#c9b89f;
			--muted:#7b6a61;
			--max-width:1100px;
		}
		*{box-sizing:border-box}
		html,body{height:100%;margin:0;font-family:'Montserrat',system-ui,Arial;padding:0;background:var(--ivory);color:var(--brown);-webkit-font-smoothing:antialiased}
		a{color:inherit}
		.container{max-width:var(--max-width);margin:0 auto;padding:24px}

		/* Header / Landing */
		.hero-landing{min-height:78vh;display:flex;align-items:center;justify-content:center;flex-direction:column;text-align:center;padding:48px 16px;background:linear-gradient(180deg,var(--ivory),var(--cream))}
		.monogram{width:120px;height:120px;border-radius:999px;border:4px solid var(--gold);display:flex;align-items:center;justify-content:center;margin:0 auto;font-family:'Playfair Display';font-size:34px;line-height:120px;padding:0;color:var(--brown);background:linear-gradient(180deg,rgba(255,255,255,0.6),rgba(255,255,255,0.2));transform:translateY(-4px)}
		.meta{letter-spacing:3px;color:var(--muted);font-size:12px;margin-top:16px}
		.names{font-family:'Playfair Display',serif;font-size:44px;color:var(--brown);margin:8px 0}
		.subtitle{color:var(--muted);max-width:700px;margin:8px auto 20px}
		.open-btn{appearance:none;border:2px solid var(--brown);background:transparent;padding:12px 20px;border-radius:30px;font-weight:600;color:var(--brown);cursor:pointer;transition:all .35s}
		.open-btn:hover{background:var(--brown);color:var(--ivory)}

		/* Main hero dark */
		.hero-dark{background:linear-gradient(180deg,var(--mocha),var(--brown));color:var(--ivory);Padding:80px 16px;text-align:center;position:relative}
		.hero-dark h2{font-family:'Playfair Display';font-size:20px;letter-spacing:2px;color:var(--gold);margin:0}
		.hero-dark h1{font-family:'Playfair Display';font-size:36px;margin:8px 0}
		.hero-decor{position:absolute;right:12%;top:-30px;width:260px;height:260px;border-radius:999px;border:1px solid rgba(255,255,255,0.06)}

		/* Save date / countdown */
		.save-date{background:var(--cream);padding:48px 16px;text-align:center}
		.save-date h3{letter-spacing:2px;color:var(--muted);margin:0}
		.event-date{font-family:'Playfair Display';font-size:24px;margin:8px 0;color:var(--brown)}
		.location{color:var(--muted);margin-bottom:12px}
		.countdown{display:flex;gap:12px;justify-content:center;margin-top:18px}
		.countdown .unit{background:rgba(0,0,0,0.04);padding:12px 14px;border-radius:8px;min-width:70px}
		.unit .num{font-family:'Playfair Display';font-size:20px}
		.unit .label{font-size:11px;color:var(--muted);margin-top:4px}

		/* Timeline */
		.timeline{padding:48px 16px}
		.timeline h3{font-family:'Playfair Display';font-size:20px;text-align:center;margin-bottom:18px}
		.timeline-list{display:flex;gap:14px;justify-content:space-between;flex-wrap:wrap}
		.timeline-item{flex:1 1 200px;background:var(--ivory);border-left:3px solid var(--gold);padding:14px;border-radius:8px}
		.timeline-item .year{font-weight:700;color:var(--mocha)}

		/* Celebration cards */
		.cards{display:flex;gap:20px;flex-wrap:wrap;padding:24px}
		.card{flex:1 1 320px;background:linear-gradient(180deg,var(--mocha),var(--brown));color:var(--ivory);padding:20px;border-radius:10px}
		.card h4{font-family:'Playfair Display';margin:0 0 6px}
		.card p{margin:4px 0;color:rgba(255,255,255,0.9)}
		.map-btn{display:inline-block;margin-top:10px;background:transparent;border:1px solid rgba(255,255,255,0.2);color:var(--ivory);padding:8px 12px;border-radius:6px;text-decoration:none}

		/* Dress code + RSVP */
		.rsvp-section{padding:28px 16px;background:var(--ivory)}
		.rsvp-grid{display:grid;grid-template-columns:1fr 1fr;gap:20px;align-items:start}
		form{background:var(--cream);padding:18px;border-radius:8px}
		label{display:block;font-size:13px;margin:8px 0 6px;color:var(--muted)}
		input[type=text],select,textarea{width:100%;padding:10px;border:1px solid #ddd;border-radius:6px;font-size:14px}
		textarea{min-height:120px}
		.submit-btn{background:var(--brown);color:var(--ivory);padding:12px 16px;border-radius:8px;border:none;cursor:pointer;margin-top:12px}

		/* Counter (people) */
		.counter{display:inline-flex;align-items:center;gap:8px}
		.counter button{width:36px;height:36px;border-radius:6px;border:1px solid #ddd;background:#fff;font-size:20px;line-height:1;cursor:pointer}
		.counter input[type=number]{width:64px;text-align:center;padding:8px;border:1px solid #ddd;border-radius:6px;font-size:14px}

		/* Footer */
		footer{padding:28px 16px;text-align:center;color:var(--muted)}

		/* Utilities & responsiveness */
		.center{text-align:center}
		@media (max-width:900px){
			.names{font-size:32px}
			.timeline-list{flex-direction:column}
			.rsvp-grid{grid-template-columns:1fr}
			.hero-decor{display:none}
		}
	</style>
</head>
<body>
	<main>
		<section class="hero-landing container" id="landing">
			<div class="monogram" data-aos="fade-up">B &amp; N</div>
			<div class="meta" data-aos="fade-up" data-aos-delay="80">TOGETHER WITH THEIR FAMILIES</div>
			<h2 class="names" data-aos="fade-up" data-aos-delay="140">Billie &amp; Nicole</h2>
			<p class="subtitle" data-aos="fade-up" data-aos-delay="200">invite you to celebrate the beginning of their forever</p>
			<button class="open-btn" id="openInvitation">OPEN INVITATION</button>
		</section>

		<section class="hero-dark" id="main" aria-label="Hero">
			<div class="hero-decor" aria-hidden="true"></div>
			<div class="container">
				<h2 data-aos="fade-up">THE WEDDING OF Billie &amp; Nicole</h2>
				<h1 data-aos="fade-up" data-aos-delay="80">A celebration of love, family, and forever.</h1>
			</div>
		</section>

		<section class="save-date" id="save-date">
			<div class="container">
				<h3 data-aos="fade-up">SAVE THE DATE</h3>
				<div class="event-date" data-aos="fade-up" data-aos-delay="60">Saturday 18 September 2027</div>
				<div class="location" data-aos="fade-up" data-aos-delay="80">Java Paragon Hotel, Surabaya</div>
				<div class="countdown" id="countdown" data-aos="fade-up" data-aos-delay="120">
					<div class="unit"><div class="num" id="days">--</div><div class="label">Days</div></div>
					<div class="unit"><div class="num" id="hours">--</div><div class="label">Hours</div></div>
					<div class="unit"><div class="num" id="minutes">--</div><div class="label">Minutes</div></div>
					<div class="unit"><div class="num" id="seconds">--</div><div class="label">Seconds</div></div>
				</div>
			</div>
		</section>

		<section class="timeline container" id="story">
			<h3 data-aos="fade-up">A love to remember - Every chapter led us here.</h3>
			<div class="timeline-list" data-aos="fade-up" data-aos-delay="80">
				<div class="timeline-item"><div class="year">2019</div><div>First met</div></div>
				<div class="timeline-item"><div class="year">2021</div><div>First date</div></div>
				<div class="timeline-item"><div class="year">2025</div><div>Engaged</div></div>
				<div class="timeline-item"><div class="year">2027</div><div>We say I do</div></div>
			</div>
		</section>

		<section class="container">
			<div class="cards">
				<div class="card" data-aos="fade-up">
					<h4>Holy Matrimony</h4>
					<p>10:00 AM — Java Paragon Hotel, Surabaya</p>
					<a class="map-btn" href="https://www.google.com/maps/search/Java+Paragon+Hotel+Surabaya" target="_blank">VIEW LOCATION</a>
				</div>
				<div class="card" data-aos="fade-up" data-aos-delay="60">
					<h4>Evening Reception</h4>
					<p>06:30 PM — Java Paragon Hotel, Surabaya</p>
					<a class="map-btn" href="https://www.google.com/maps/search/Java+Paragon+Hotel+Surabaya" target="_blank">VIEW LOCATION</a>
				</div>
			</div>
		</section>

		<section class="rsvp-section" id="rsvp">
			<div class="container">
				<div class="center" data-aos="fade-up"><h3>Dress Code</h3><p class="location">Smart Formal — Gentlemen in suits, ladies in evening dresses.</p></div>

				<div class="rsvp-grid" data-aos="fade-up" data-aos-delay="80">
					<div>
						<h3>RSVP & Confirmation</h3>
						<form id="rsvpForm">
							<label for="name">Full Name</label>
							<input type="text" id="name" name="name" placeholder="Your name" required>

							<label for="attendance">Attendance</label>
							<select id="attendance" name="attendance">
								<option value="attending">Attending</option>
								<option value="not_attending">Not Attending</option>
							</select>

							<label for="food">Food Preference</label>
							<select id="food" name="food">
								<option>No Preference</option>
								<option>Vegetarian</option>
								<option>Halal</option>
							</select>
								<label for="Pax">Number of Pax?</label>
								<div class="counter" role="group" aria-label="Number of Pax">
									<button type="button" class="decrease" aria-label="Decrease">−</button>
									<input type="number" id="Pax" name="Pax" value="1" min="1" max="10" />
									<button type="button" class="increase" aria-label="Increase">+</button>
								</div>

							<label for="message">Leave a little note...</label>
							<textarea id="message" name="message" placeholder="Write your wishes here..."></textarea>

							<button class="submit-btn" type="submit">CONFIRM ATTENDANCE</button>
						</form>
					</div>

					<div>
						<h3>Practical Info</h3>
						<p><strong>Venue:</strong> Java Paragon Hotel, Surabaya</p>
						<p><strong>Parking:</strong> Valet available</p>
						<p><strong>Contact:</strong> +62 812-3456-7890</p>
					</div>
				</div>
			</div>
		</section>

		<footer>
			<div class="container">
				<div class="monogram" style="display:inline-block;">B &amp; N</div>
				<p style="margin-top:12px">With love, Billie &amp; Nicole — September 18, 2027 — Surabaya</p>
			</div>
		</footer>
	</main>

	<audio id="bgMusic" src="" preload="none"></audio>

<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
	<script>
		AOS.init({duration:700, once:true});

		// Smooth scroll + music play
		const openBtn = document.getElementById('openInvitation');
		const mainSection = document.getElementById('main');
		const bgMusic = document.getElementById('bgMusic');

		openBtn.addEventListener('click', ()=>{
			mainSection.scrollIntoView({behavior:'smooth'});
			if(bgMusic && bgMusic.src){
				bgMusic.play().catch(()=>{/* playback blocked until user gesture */});
			}
		});

		// Countdown Timer
		const target = new Date(2027, 8, 18, 17, 0, 0); // 18 Sep 2027
		function updateCountdown(){
			const now = new Date();
			const diff = target - now;
			if(diff <= 0){
				document.getElementById('days').textContent = '0';
				document.getElementById('hours').textContent = '0';
				document.getElementById('minutes').textContent = '0';
				document.getElementById('seconds').textContent = '0';
				clearInterval(timerId);
				return;
			}
			const secs = Math.floor(diff / 1000);
			const days = Math.floor(secs / 86400);
			const hours = Math.floor((secs % 86400) / 3600);
			const minutes = Math.floor((secs % 3600) / 60);
			const seconds = secs % 60;
			document.getElementById('days').textContent = days;
			document.getElementById('hours').textContent = String(hours).padStart(2, '0');
			document.getElementById('minutes').textContent = String(minutes).padStart(2, '0');
			document.getElementById('seconds').textContent = String(seconds).padStart(2, '0');
		}
		const timerId = setInterval(updateCountdown, 1000);
		updateCountdown();

		// People counter (+ / -) logic
		(function(){
			const dec = document.querySelector('.counter .decrease');
			const inc = document.querySelector('.counter .increase');
			const input = document.getElementById('Pax');
			if(!input) return;
			const min = parseInt(input.min || '1', 10);
			const max = parseInt(input.max || '10', 10);
			dec.addEventListener('click', ()=>{
				let v = parseInt(input.value || '1', 10);
				if(v > min) input.value = v - 1;
			});
			inc.addEventListener('click', ()=>{
				let v = parseInt(input.value || '1', 10);
				if(v < max) input.value = v + 1;
			});
			input.addEventListener('input', ()=>{
				let v = parseInt(input.value || String(min), 10);
				if(isNaN(v) || v < min) input.value = min;
				else if(v > max) input.value = max;
			});
		})();

		// ==========================================
		// PENGIRIMAN FORM RSVP KE GOOGLE SHEETS
		// ==========================================
		
		const SCRIPT_URL = 'https://script.google.com/macros/s/AKfycby0WOWDRl65ZrTMQJ3E51gCK8pA77CGHhDfKm6mHN5oCUcxrYefluxIyiYZUpuGgWCO7w/exec';

		const form = document.getElementById('rsvpForm');
		const submitBtn = form.querySelector('.submit-btn');

		form.addEventListener('submit', (e) => {
			e.preventDefault();

			// Pengecekan disesuaikan agar tidak memblokir URL Anda
			if (SCRIPT_URL === 'PASTE_WEB_APP_URL_ANDA_DI_SINI' || !SCRIPT_URL) {
				alert('Silakan masukkan SCRIPT_URL Apps Script Anda terlebih dahulu!');
				return;
			}

			const formData = {
				name: document.getElementById('name').value.trim(),
				attendance: document.getElementById('attendance').value,
				food: document.getElementById('food').value,
				pax: document.getElementById('Pax').value,
				message: document.getElementById('message').value.trim()
			};

			const originalBtnText = submitBtn.textContent;
			submitBtn.textContent = 'Sending...';
			submitBtn.disabled = true;

			fetch(SCRIPT_URL, {
				method: 'POST',
				mode: 'no-cors',
				headers: {
					'Content-Type': 'application/json'
				},
				body: JSON.stringify(formData)
			})
			.then(() => {
				alert('Terima kasih, ' + formData.name + '! Konfirmasi RSVP Anda berhasil disimpan.');
				form.reset();
				document.getElementById('Pax').value = '1';
			})
			.catch((error) => {
				console.error('Error:', error);
				alert('Maaf, terjadi kesalahan saat mengirim data. Silakan coba lagi.');
			})
			.finally(() => {
				submitBtn.textContent = originalBtnText;
				submitBtn.disabled = false;
			});
		});
	</script>
</body>
</html>


