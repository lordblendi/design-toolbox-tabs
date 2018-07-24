# Design Toolbox Tabs

Tabs component of the TenForce design toolbox.

## CSS

This component is using [one](https://github.com/tenforce/design-toolbox-tabs/blob/master/docs/sass/style.scss) CSS file.

## HTML structure

The Design documentation was built in Jekyll using SASS and Liquid.

```html
<div class="toolbox-tabs">
  <div class="toolbox-tabs-nav">
    <div class="toolbox-tabs-nav__slide toolbox-tabs-nav__slide--left toolbox-tabs-nav__slide--hidden">
      <span class="toolbox-tabs-nav__slideShadow"></span>
      <span class="toolbox-tabs-nav__slideArrow">←</span>
      <span class="toolbox-tabs-nav__slideCounter">1</span>
    </div>
    <ul>
      <span class="toolbox-tabs-nav__linkBar"></span>
      <li>
        <a href="#" class="toolbox-tabs-nav__link {{activeTab}}"><span>{{tab}}</span></a>
      </li>
    </ul>
    <div class="toolbox-tabs-nav__slide toolbox-tabs-nav__slide--right">
      <span class="toolbox-tabs-nav__slideShadow"></span>
      <span class="toolbox-tabs-nav__slideArrow">→</span>
      <span class="toolbox-tabs-nav__slideCounter">9</span>
    </div>
  </div>
  <div class="toolbox-tabs-panels">
    <div class="toolbox-tabs-panels__panel">
      {{tab}}
    </div>
  </div>
</div>
```

The wrapper is `toolbox-tabs`, and it includes two children: `toolbox-tabs-nav` and `toolbox-tabs-panels`.

The navigation contains a slider on both sides with a shadow, an arrow and a counter (of how many items are hidden). Between the sliders, you have a ul of navigation links. The ul also contains a linkBar span, that is the line that gets animated when clicking on another tab.

The panels just contains multiple children divs, for each panel.

See the following files:
- [tabs](https://github.com/tenforce/design-toolbox-tabs/blob/master/docs/_includes/components/toolbox-tabs.html)
- [nav](https://github.com/tenforce/design-toolbox-tabs/blob/master/docs/_includes/components/toolbox-tabs-nav.html)
- [panels](https://github.com/tenforce/design-toolbox-tabs/blob/master/docs/_includes/components/toolbox-tabs-panels.html)


## Usage
### Links to CSS files
- main CSS
  - [built](https://tenforce.github.io/design-toolbox-tabs/sass/style.css)
  - [raw](https://github.com/tenforce/design-toolbox-tabs/blob/master/docs/sass/style.scss)

### Jekyll
Add [the content of this file](https://github.com/tenforce/design-toolbox-tabs/tree/master/docs/import/include-tabs.html) to the another Jekyll project to include files from this project.

## Dependencies
- [Tailwind v0.6.4](https://tailwindcss.com)
- [TenForce default CSS](https://github.com/tenforce/design-toolbox-default-css)
- [jQuery (for javascript)](https://jquery.com)
