<!-- <details style="display: none" class="details-reset details-overlay details-overlay-dark">
  <summary class="btn" aria-haspopup="dialog" role="button">Dark Mode</summary>
  <div>In Development...</div>
</details> -->

![](https://suhay.github.io/suhay/images/github.svg)

<!-- 
![](https://suhay.github.io/suhay/images/text.svg)

## Hacking your Github Profile's README:

<details class="details-overlay">
  <summary class="btn">Why?</summary>
  <div class="border p-3 mt-2" markdown="1">  
  
Why not?  

When it was discovered that Github had introduced the __secret__ repository trick for upgrading your profile's landing page, I, like many of my fellow developers, opened our favorite markdown editors, popped a tray of pizza roles into the toaster oven, and then went to town on crafting the greatest README file this side of the internet has ever seen. It was a true work of art; animated gifs, emojis as punctuation, artfully placed horizontal rules. I was on :fire:. But something was missing.  

This wasn't anything new we haven't already been putting in our READMEs for years, and nobody was reading them then so why would they now? Well, outside of basic troubleshooting and install instructions, but I wanted more than a TLDR section, I needed more...  

### Dissembling the Content-Security-Policy

Unfortunately, for us, Github has a pretty airtight CSP which blocks. With `script-src` locked down to `github.githubassets.com`, we're not going to be able to load in any 3rd parties which is going to drastically limit what we can do with JavaScript and manipulating the page directly. `media-src` is set to `'none'` so `<audio>` and `<video>` are out, and with them my dreams of turning my page into a nightmarish 90s style MySpace clone. And with `frame-src` only allowing source content from `render.githubusercontent.com`, my hopes of hacking my README page were quickly evaporating. Unless I wanted to use nothing but [Math Equations](https://render.githubusercontent.com/render/math?math=e^{i%20\pi}%20=%20-1).  

So what was learned?

- [x] script-src 
- [x] frame-src 
- [x] media-src 
- [ ] style-src
- [ ] img-src 
- [ ] form-action 

## `<svg>`: Excuse me streamer, it's pronounced "s-vij" with a soft "g"...

It looks like our main vector (pun) is going to be trying to inject a `<style>` block directly into the Markdown since the CSP is explicitly allowing `'unsafe-inline'`, but I'm pretty sure Github is escaping those out, so I didn't spend too much time trying to battle their regex just yet. The next thing to try was getting one inside of an `<svg>` and uploading it to the repo while turning the `/docs` folder into a Github Pages directory. This step may not have been necessary, but I wanted to be doubley sure that the file was being served off of a Github owned domain. As a partial success, the `<style>` block wasn't getting escaped into oblivion, but the SVG file was coming in as an `<img>` so I wasn't able to directly reach into my styles nor was I able to use any of the available within the page. In side the `<svg>`, so far, was where we had the most control, so at least we had a fallback plan.  

## Priming with @primer

More Coming...  
  </div>
</details> -->



<!-- https://primer.style/css/utilities/details -->
