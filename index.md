<!-- .slide: data-background="images/background/00.svg" -->

# Web Accessibility Best Practices

<p class="author">
    Kelly Hutchins<br>
    Tao Zhang
</p>

<p id="slidesInfo">Jan 23, 2019 · Esri GeoDev Webinar</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <img id="gotowebinar" src="images/gotowebinar.png" alt="Screenshots of Gotowebinar panel">
</p>



<!-- .slide: data-background="images/background/00.svg" -->

# Web Accessibility Best Practices

<p class="author">
    Kelly Hutchins<br>
    Tao Zhang
</p>

<p id="slidesInfo">Jan 23, 2019 · Esri GeoDev Webinar</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="centertitle">What is accessibility?</h2>

Make content usable for everyone regardless of abilities



---
<!-- .slide: data-background="images/background/01.svg" -->

## Disability statistics

- 15% of world population lives with some form of disability
- In the US, 1 in 5 adults has a disability
- 8% of male have some degree of color blindness



---
<!-- .slide: data-background="images/background/01.svg" -->

<h3 class="centertitle">Wide range of disabilities</h2>

<p class="centerp">
    <img id="msinclusive" src="images/MS_inclusive.jpg" alt="Infographic showing a wide range of disabilities">
</p>
<p id="mssource"><a href="https://www.microsoft.com/en-us/design/inclusive">Inclusive Design at Microsoft</a></p>



---
<!-- .slide: data-background="images/background/01.svg" -->

## Why is accessibility important?

- The ADA and Section 508
- People with different abilities should have equal access to the web
- Good accessibility is good user experience



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="twocoltitle">How is Esri doing?</h2>

<div class="twocol">
    <ul class="leftcol">
        <li>Reviewing products internally for compliance</li>
        <li>Fixing accessibility issues</li>
        <li>Working accessibility into new features</li>
        <li>Sharing knowledge and best practices</li>
    </ul>
    <img class="rightcol" src="images/storymap-announcement2.png" alt="Screenshots of GeoNet accessibility group and announcement of new accessibility features in Story Maps"/>
</div>



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="twocoltitle">WCAG</h2>

Web Content Accessibility Guidelines



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <img src="images/wcag.png" alt="Screenshots of WCAG 2.0 and 2.1 official docs">
</p>


---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="centertitle">Overview of WCAG 2.0</h2>

<p class="centerp">
    <img id="wcagoverview" src="images/wcag_overview.png" alt="Overview diagram of WCAG principles, success criteria, and levels">
</p>


---
<!-- .slide: data-background="images/background/01.svg" -->

## What we will cover today

- Focus and tab order
- Color and color contrast
- Text alternatives
- Map for non-sighted users
- A DIY accessibility test process



---
<!-- .slide: data-background="images/background/01.svg" -->

## Our focus today

- How to get started in accessibility
- Simple and effective actions
- Finding issues before working with the code



---
<!-- .slide: data-background="images/background/01.svg" -->

## Focus and tab order

<ul>
    <li class="fragment"><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/navigation-mechanisms-focus-visible.html">WCAG 2.4.7</a>: Interactive elements should have clear focus.</li>
    <li class="fragment"><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/content-structure-separation-sequence.html">WCAG 1.3.2</a>: Navigation (tab) order should be logical and intuitive.</li>
    <li class="fragment"><a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation-keyboard-operable.html">WCAG 2.1.1</a>: Keyboard users should be able to use functionalities using keyboard only.</li>
    <li class="fragment"><a href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/keyboard-operation-trapping.html">WCAG 2.1.2</a>: Content does not "trap" keyboard focus within subsections.</li>
</ul>



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <a href="demos/focus_and_tab_order/index.html">Demo: Focus and tab order</a>
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <a href="images/modal_example.gif">Demo: Focus trap in dialog</a>
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <a href="https://arcgis103.esri.ca/WCAG-Configurable-Template-Test/?appid=e951691e3893444ea64e7c29d086e30c">Example: Accessible App of Electric Charging Stations</a>
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

## Test focus and tab order

- Tab through page to verify all interactive elements have focus
- Focus order matches intended reading order
- Interact with all links and controls using only keyboard
- No keyboard trap except for modals
- Off-screen/invisible content does not receive focus



---
<!-- .slide: data-background="images/background/01.svg" -->

## Color and color contrast

<ul>
    <li class="fragment"><a href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-without-color.html">WCAG 1.4.1</a>: Color is not the only visual means of conveying information.</li>
    <li class="fragment"><a href="http://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html">WCAG 1.4.3</a>: Text needs to have contrast ratio of at least 4.5:1.</li>
</ul>



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <a href="demos/color-contrast/index.html">Demo: Color and color contrast</a>
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="centertitle">White text on colored background</h2>

<p class="centerp">
    <img src="images/color-example-1.png" alt="Example of white text on light colored background">
</p>
<hr>
<p class="centerp">
    <img class="fragment" src="images/color-example-2.png" alt="Example of white text on dark colored background">
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="centertitle">Flipping the contrast</h2>

<p class="centerp">
    <img src="images/color-example-3.png" alt="Example of black text on light colored background">
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

## Test color and color contrast

- Look for content differentiated by color only
- Use a [contrast ratio calculator](https://contrast-ratio.com/)
- Review color contrast issues reported by automated test tool ([aXe](https://chrome.google.com/webstore/detail/axe/lhdoppojpmngadmnindnejefpokejbdd))



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="twocoltitle">Text alternatives</h2>

<p>
    <a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/text-equiv-all.html">WCAG 1.1.1</a>: Non-text content has text alternative.
</p>
<p>
    If image is decorative, use `alt=""`.
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <ul>
    <li><a href="https://developers.arcgis.com/javascript/latest/sample-code/widgets-basemapgallery/live/index.html">Demo: Text alternative - empty alt</a></li>
     <li><a href="https://story.maps.arcgis.com/apps/MapJournal/index.html?appid=2b1c793f464b4cd2944a0b9700c0dc48">Demo: Text alternative - descriptive</a></li>
     </ul>
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

## Write effective alternate text

- Think about how users will be doing with the information
- Be accurate in presenting the content in images
- Be succinct
- No need to use the phrase "image of ..." to describe images



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="centertitle">Map for non-sighted users</h2>

<p class="centerp">
    <img id="a11ymap" src="images/a11y-map.png" alt="Screenshot of the accessible map prototype by Esri">
</p>

<p class="source">GitHub repo: <a href="https://github.com/Esri/a11y-map">https://github.com/Esri/a11y-map</a></p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<video controls>
    <source src="images/a11y-map-demo.mp4"  type="video/mp4">
</video>

<p class="source"><a href="https://github.com/jimmieego/Web-Accessibility-Best-Practices/blob/masterimages/a11y-map-demo.mp4">Video link</a></p>



---
<!-- .slide: data-background="images/background/01.svg" -->

## DIY accessibility test

<ol>
    <li>Automated test</li>
    <li>Keyboard test</li>
    <li>Screen reader test</li>
    <li>Color test</li>
</ol>



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2>Automated test with <a href="https://www.deque.com/products/axe/">aXe</a></h2>

<p class="centerp">
    <img id="axe" src="images/axe.png" alt="Screenshots of aXe extension in Chrome"/>
</p>

<ul>
    <li>Tests rendered page in browser</li>
    <li>Less false positives</li>
    <li>Accessible</li>
</ul>



---
<!-- .slide: data-background="images/background/01.svg" -->

<p class="centerp">
    <a href="demos/map-demo/index.html">Demo: Automated test using aXe</a>
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="centertitle">Keyboard test</h2>

<p class="centerp">
    <img id="axe" src="images/keyboard.png" alt="List of keyboard actions"/>
</p>



---
<!-- .slide: data-background="images/background/01.svg" -->

<h2 class="centertitle">Screen reader</h2>

| OS      | Screen reader | Browser |
|---------|---------------|---------|
| MacOS   | [VoiceOver](https://www.apple.com/accessibility/mac/vision/)     | Safari  |
| Windows | [NVDA](https://www.nvaccess.org/)          | Firefox |
| Windows | [JAWS](http://www.freedomscientific.com/Products/Blindness/JAWS)          | IE/Edge |



---
<!-- .slide: data-background="images/background/01.svg" -->

## Screen reader basics

- [A11ycasts: VoiceOver](https://youtu.be/5R-6WvAihms)
- [A11ycasts: NVDA](https://youtu.be/Jao3s_CwdRU)



---
<!-- .slide: data-background="images/background/01.svg" -->

## Color test

- Automated color contrast test results may need manual verification
- Look for information differentiated only by color



---
<!-- .slide: data-background="images/background/02.svg" -->

## Additional resources

- [MDN: Accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility)
- [Google Developers Web Fundamentals: Accessibility](https://developers.google.com/web/fundamentals/accessibility/)
- [The A11Y Project](https://a11yproject.com/)
- [GeoNet: Accessibility](https://community.esri.com/groups/accessibility)



---
<!-- .slide: data-background="images/background/02.svg" -->

### Questions?

<p class="centerp source">Slides: https://arcg.is/1a910T</p>
