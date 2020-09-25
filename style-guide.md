---
title: Style Guide
subtitle: >-
  The style guide provides you with a blueprint of default post and page styles.
  The style guide is also a great reference for suggested typographic treatment
  and styles for your content.
layout: page
---

**This is a paragraph**. Pellentesque habitant morbi *tristique senectus et netus et malesuada* fames ac turpis egestas. Vestibulum [tortor quam](https://www.google.com), feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo. Quisque sit <mark>amet est et sapien ullamcorper</mark> pharetra. Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi.

# This is an H1

Quisque facilisis erat a dui. Nam malesuada ornare dolor. Cras gravida, this is marked text ornare, erat elit consectetuer erat, id egestas pede nibh eget odio. Proin tincidunt, velit vel porta elementum, magna diam molestie sapien, non aliquet massa pede eu diam. Aliquam iaculis. Fusce et ipsum et nulla tristique facilisis.

## This is an H2

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Morbi commodo, ipsum sed pharetra gravida, orci magna rhoncus neque, id pulvinar odio lorem non turpis. Nullam sit amet enim. Suspendisse id velit vitae ligula volutpat condimentum. Aliquam erat volutpat. Sed quis velit. Nulla facilisi. Nulla libero.

### This is an H3

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Morbi commodo, ipsum sed pharetra gravida, orci magna rhoncus neque, id pulvinar odio lorem non turpis. Nullam sit amet enim. Suspendisse id velit vitae ligula volutpat condimentum. Aliquam erat volutpat. Sed quis velit. Nulla facilisi. Nulla libero.

#### This is an H4

Quisque facilisis erat a dui. Nam malesuada ornare dolor. Cras gravida, diam sit amet rhoncus ornare, erat elit consectetuer erat, id egestas pede nibh eget odio. Proin tincidunt, velit vel porta elementum, magna diam molestie sapien, non aliquet massa pede eu diam. Aliquam iaculis.

## Quoting

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Morbi commodo, ipsum sed pharetra gravida, orci magna rhoncus neque, id pulvinar odio lorem non turpis. Nullam sit amet enim. Suspendisse id velit vitae ligula volutpat condimentum. Aliquam erat volutpat. Sed quis velit. Nulla facilisi. Nulla libero.

>&ldquo;Creativity is allowing yourself to make mistakes. Design is knowing which ones to keep.&rdquo;

Nunc a lorem tellus. Aenean eu auctor purus. Cras pulvinar, nunc at sagittis dignissim, orci elit auctor leo, et consectetur est turpis a nunc. Vivamus in faucibus felis. Aenean rutrum magna at ex auctor, congue efficitur ligula feugiat. Proin a egestas arcu.

<hr />

## Unordered Lists

+ Donec non tortor in arcu mollis feugiat
+ Lorem ipsum dolor sit amet, consectetuer adipiscing elit

## Ordered Lists

1. Donec non tortor in arcu mollis feugiat
2. Lorem ipsum dolor sit amet, consectetuer adipiscing elit

## Code Blocks

Blocks of code are either fenced by lines with three back-ticks, or are indented with four spaces.

```
<!-- Some example CSS code -->
body {
  color:red;
}
```

## Tables

<table>
    <caption>Table with thead, tfoot, and tbody</caption>
  <thead>
    <tr>
      <th>Header content 1</th>
      <th>Header content 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Body content 1</td>
      <td>Body content 2</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Footer content 1</td>
      <td>Footer content 2</td>
    </tr>
  </tfoot>
</table>

## Call to action

Defined from an event as:

```yaml 
actions:
  text: Registration for attendees is now open!
  url: https://github.com
  action: Register
  background: accent
```

Where background can be any of: `dark`, `accent`, `primary`, `secondary`, `white` or `gradient`.

<section id="call-to-action" class="block cta-block bg-accent outer">
  <div class="inner-large">
    <div class="grid">
      <div class="cell block-content">
        <h4 class="block-title">This is a call to action</h4>
      </div><!-- .block-content -->
      <p class="cell block-buttons">
        <a href="{{page.actions.url}}" class="button secondary" target="_blank">Click here</a>
      </p>
    </div><!-- .grid -->
  </div><!-- .inner -->
</section><!-- .cta -->