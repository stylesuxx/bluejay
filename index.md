## Project Summary
Bluejay is an open source fork of [BLHeli_S](https://github.com/bitdump/BLHeli).

It is still in early development and further testing is needed before it should be used for serious flight.
If you want to help testing it any feedback you can provide is greatly appreciated!

### Current Features

- Digital signal protocol: DShot 300 and 600
- Bidirectional DShot: RPM telemetry
- Selectable PWM frequency: 24, 48 and 96 kHz
- PWM dithering: 10-bit effective throttle resolution

## Flashing ESCs
The Bluejay firmware can be flashed to BLHeli_S compatible ESCs using BLHeli Configurator.

All releases can be found in the [releases](https://github.com/mathiasvr/bluejay/releases) section.

Release files use a naming convention similar to BLHeli: `{T}_{M}_{D}_{P}_{V}.hex`.

|---|--------------------|-------------------------------------------------------|
| T | `A` - `W`          | Target ESC layout                                     |
| M | `L` or `H`         | MCU type: `L` (BB1 24MHz), `H` (BB2 48MHz)            |
| D | `0` - `90`         | Deadtime (`0` *only* for ESCs with built-in deadtime) |
| P | `24`, `48` or `96` | PWM frequency [kHz]                                   |
| V | eg. `0.4.0`        | Bluejay version                                       |


<div id="disqus_thread"></div>
<script>
var disqus_config = function () {
    this.page.url = '{{ page.url }}';
    this.page.identifier = '{{ page.url }}';
};
(function() { // DON'T EDIT BELOW THIS LINE
    var d = document, s = d.createElement('script');
    s.src = 'https://bluejay-3.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
