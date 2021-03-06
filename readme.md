## Console Fright Night

Give someone an Audio fright... or welcome, when they open the web inspector/console on your website. (using safari/chrome ... sorry!)

#### Instructions

`Console Fright Night` is a stand alone library (no jquery, or the likes) so usage is pretty straight forward. You'll need to include `CFN.js` to your page, and create a new instance of `CFN`.

#### Usage

`Console Fright Night (CFN)` lives entirely within the js realm, which makes things fairly simple to use.

```html
<script>
// Elevator script included on the page, already.

// You can init the script, by calling.
window.onload = function() {
  new CFN({src: "path-to-your-audio-file.mp3"});
}

</script>
```

#### But How
`CFN` defines a custom "getter" to an audio element, which is then constantly logged to the console. When the browser is actually open, this getter will be triggered, allowing us to detect that the console is open. This happens on lines 31 - 33 of `cfn.js`.

Because of these console checks, it will look like your console is being spammed, but thats how it works. Not much else we can do there.

#### License

Console Fright Night is covered by the MIT License.

Copyright (C) 2016 ~ [Tim Holman](http://tholman.com) ~ timothy.w.holman@gmail.com