<body><article class="h-entry">
<header>
<h1 class="p-name">This Election — AMBIENT NONSENSE</h1>
</header>
<section data-field="body" class="e-content">
<section name="739d" class="section section--body section--first section--last"><div class="section-divider layoutSingleColumn"><p name="9775" id="9775" class="graf graf--p graf-after--h3">These printers use Particle’s Photon, <a href="https://medium.com/u/c9914184139c" data-href="https://medium.com/u/c9914184139c" data-anchor-type="2" data-user-id="c9914184139c" data-action="show-user-card" data-action-type="hover" class="markup--user markup--p-user" target="_blank">adafruit industries</a>’s Thermal Printers and <a href="https://medium.com/u/10ab0b09ba3e" data-href="https://medium.com/u/10ab0b09ba3e" data-anchor-type="2" data-user-id="10ab0b09ba3e" data-action="show-user-card" data-action-type="hover" class="markup--user markup--p-user" target="_blank">IFTTT</a>’s platform to print in real time everything the candidates say online:</p></div><div class="section-inner sectionLayout--fullWidth"><figure name="9870" id="9870" class="graf graf--figure graf--layoutFillWidth graf-after--p"><div class="aspectRatioPlaceholder is-locked"><div class="aspectRatioPlaceholder-fill" style="padding-bottom: 60.8%;"></div><img class="graf-image" data-image-id="1*r79ZKNYNCncbUFa_Vd_y3w.jpeg" data-width="4926" data-height="2993" data-is-featured="true" src="https://cdn-images-1.medium.com/max/2000/1*r79ZKNYNCncbUFa_Vd_y3w.jpeg"></div></figure></div><div class="section-inner sectionLayout--outsetColumn"><figure name="5609" id="5609" class="graf graf--figure graf--layoutOutsetCenter graf-after--figure"><div class="aspectRatioPlaceholder is-locked" style="max-width: 1020px; max-height: 1360px;"><div class="aspectRatioPlaceholder-fill" style="padding-bottom: 133.29999999999998%;"></div><img class="graf-image" data-image-id="1*Z3s9rmpouPfL9v8r37ACGw.jpeg" data-width="2448" data-height="3264" src="https://cdn-images-1.medium.com/max/2000/1*Z3s9rmpouPfL9v8r37ACGw.jpeg"></div></figure></div><div class="section-inner layoutSingleColumn"><p name="879e" id="879e" class="graf graf--p graf-after--figure">It’s not so much about what they tweet, in this configuration. It’s about the piles. The expression of information / propaganda in piles, on both sides. There’s something relaxing about it.</p></div><div class="section-inner sectionLayout--outsetRow" data-paragraph-count="2"><figure name="b594" id="b594" class="graf graf--figure graf--layoutOutsetRow is-partialWidth graf-after--p" style="width: 50%;"><div class="aspectRatioPlaceholder is-locked"><div class="aspectRatioPlaceholder-fill" style="padding-bottom: 66.7%;"></div><img class="graf-image" data-image-id="1*HCdbGwZKJUK3ts7hvYCxEQ.jpeg" data-width="5760" data-height="3840" src="https://cdn-images-1.medium.com/max/1200/1*HCdbGwZKJUK3ts7hvYCxEQ.jpeg"></div></figure><figure name="f4bd" id="f4bd" class="graf graf--figure graf--layoutOutsetRowContinue is-partialWidth graf-after--figure" style="width: 50%;"><div class="aspectRatioPlaceholder is-locked"><div class="aspectRatioPlaceholder-fill" style="padding-bottom: 66.7%;"></div><img class="graf-image" data-image-id="1*51VrLn_y0ApJWs64ArnAyQ.jpeg" data-width="5760" data-height="3840" src="https://cdn-images-1.medium.com/max/1200/1*51VrLn_y0ApJWs64ArnAyQ.jpeg"></div></figure></div><div class="section-inner layoutSingleColumn"><h2 name="938a" id="938a" class="graf graf--h3 graf-after--figure">Diagram</h2><figure name="694a" id="694a" class="graf graf--figure graf-after--h3"><div class="aspectRatioPlaceholder is-locked" style="max-width: 700px; max-height: 695px;"><div class="aspectRatioPlaceholder-fill" style="padding-bottom: 99.2%;"></div><img class="graf-image" data-image-id="1*JdCxKtdP8zjxkNCRhov4lQ.png" data-width="1686" data-height="1673" src="https://cdn-images-1.medium.com/max/1600/1*JdCxKtdP8zjxkNCRhov4lQ.png"></div></figure><p name="95f5" id="95f5" class="graf graf--p graf-after--figure">The printer is connected to a 9V wall wart (2.0A, if it’s too low the text will come out as gray). You can power the Photon directly with a 3.3–7 power supply or with 5V via the micro usb port.</p><h2 name="bcd4" id="bcd4" class="graf graf--h3 graf-after--p">IFTTT Sample recipe</h2><figure name="6027" id="6027" class="graf graf--figure graf-after--h3"><div class="aspectRatioPlaceholder is-locked" style="max-width: 700px; max-height: 708px;"><div class="aspectRatioPlaceholder-fill" style="padding-bottom: 101.1%;"></div><img class="graf-image" data-image-id="1*6_H99aAbJGO-FOOZuLHjpg.png" data-width="1426" data-height="1442" src="https://cdn-images-1.medium.com/max/1600/1*6_H99aAbJGO-FOOZuLHjpg.png"></div></figure><p name="cb2f" id="cb2f" class="graf graf--p graf-after--figure">This <a href="http://ifttt.com/" data-href="http://ifttt.com/" class="markup--anchor markup--p-anchor" target="_blank">IFTTT Recipe</a> creates a <a href="https://docs.particle.io/reference/firmware/photon/#particle-subscribe-" data-href="https://docs.particle.io/reference/firmware/photon/#particle-subscribe-" class="markup--anchor markup--p-anchor" target="_blank">particle event</a> for each tweet generated from Donald Trump (and another recipe does the same for Hillary).</p><blockquote name="9c51" id="9c51" class="graf graf--pullquote graf-after--p">If Tweet then Particle Event</blockquote><p name="32a1" id="32a1" class="graf graf--p graf-after--pullquote">The particle is running code that triggers on every new event of that type, and prints it out in physical space (using <a href="https://medium.com/u/c9914184139c" data-href="https://medium.com/u/c9914184139c" data-anchor-type="2" data-user-id="c9914184139c" data-action="show-user-card" data-action-type="hover" class="markup--user markup--p-user" target="_blank">adafruit industries</a>’s <a href="https://learn.adafruit.com/mini-thermal-receipt-printer/microcontroller" data-href="https://learn.adafruit.com/mini-thermal-receipt-printer/microcontroller" class="markup--anchor markup--p-anchor" target="_blank">Thermal Printing library</a>.</p>
<h2 name="3b38" id="3b38" class="graf graf--h3 graf-after--p">Code Example</h2>
<p name="95d4" id="95d4" class="graf graf--p graf-after--h3">See the example on github</p><figure name="708f" id="708f" class="graf graf--figure graf--iframe graf-after--p graf--last"></figure></div></div></section>
</section>
</article>

</body></html>
