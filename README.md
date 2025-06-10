# Bytebeat Converter
<h2>Info.</h2>
A Bytebeat/Signed Bytebeat, Floatbeat converter
<h2>Example: From: Floatbeat, To: Bytebeat</h2>
<h3>Input:</h3> <code>noi=(x,a)=>sin(x/9E3*x*x*x)/256*a,kick=sin(1.6**(-t/512%32+8))/2,snare=noi(int(t/3)*'01'[t>>14&1],-(t/128%128)+128)/3,hihat=noi(t,16-sqrt(-t&4095)/1.5),mel=min(max(atan(tan(t*[1,4,1,4,1.05,4,1.05,4][t>>13&7]*'10'[t>>12&1]/2/41)^sin(t/41)),-1),1)/((t/512&7)+3),bas=asin(sin(t*[1,1.05,1,1.05,0,1,1.05,1][t>>14&7]/41))/4,(kick+snare+hihat+mel+bas)/1.5</code>                                                                                                                                                                                                                                                                                                                                 <h3>Output:</h3><code>Math.max(0, Math.min(255, ((noi=(x,a)=>sin(x/9E3*x*x*x)/256*a,kick=sin(1.6**(-t/512%32+8))/2,snare=noi(int(t/3)*'01'[t>>14&1],-(t/128%128)+128)/3,hihat=noi(t,16-sqrt(-t&4095)/1.5),mel=min(max(atan(tan(t*[1,4,1,4,1.05,4,1.05,4][t>>13&7]*'10'[t>>12&1]/2/41)^sin(t/41)),-1),1)/((t/512&7)+3),bas=asin(sin(t*[1,1.05,1,1.05,0,1,1.05,1][t>>14&7]/41))/4,(kick+snare+hihat+mel+bas)/1.5) + 1.0) * 127.5))</code>

<h2>Upcoming Data</h2>
I am later on going to work on making funcbeat work, add a minibaker/deminibaker, and add an audio to pcm string
