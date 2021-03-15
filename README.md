
<div align="center">
 <img alt="Logo" src="https://github.com/pycon-mentored-sprints/digital-assets/blob/master/logos/MS_logo_white.png?raw=true" width="300" />
</div>
<br>

<div align="center">
<h1><a href="https://mentored-sprints.dev">mentored-sprints.dev</a></h1>
</div>

[![License](https://img.shields.io/badge/License-BSD%203--Clause-gray.svg?colorA=2D2A56&colorB=7A76C2&style=flat.svg)](https://opensource.org/licenses/BSD-3-Clause)

[![Netlify Status](https://api.netlify.com/api/v1/badges/22aa2846-c490-494e-b625-50a322ecc94f/deploy-status)](https://app.netlify.com/sites/amazing-cray-35954b/deploys)

- [💻 Development](#-development)
  - [Running this Site Locally](#running-this-site-locally)
  - [📝 Adding content to the site](#-adding-content-to-the-site)
    - [📅 Events](#-events)
    - [:pencil: Website section](#-website-section)
  - [:book: Style-guide](#-style-guide)
    - [:art: Colours](#-colours)
    - [:bookmark: Section colours](#-section-colours)
- [:raised_hands: Contributing](#-contributing)
- [:book: License](#-license)

This repository contains the source code for [mentored-sprints.dev](mentored-sprints.dev), which is the main website for Mentored Sprints.

If you are looking for the source for the [Community Handbook](https://github.com/pycon-mentored-sprints/community-handbook), head to [https://github.com/pycon-mentored-sprints/community-handbook](https://github.com/pycon-mentored-sprints/community-handbook).

## 💻 Development

### Running this Site Locally

This website is build using Jekyll and served through Netlify. If you want to make changes to the site, follow these steps to work on this on your local computer.

1. Install a full [Ruby development environment](https://jekyllrb.com/docs/installation/)

2. Install Jekyll and Bundler

        gem install jekyll bundler

3. Install dependencies from Gemfile:

        bundle install
4. Build the site and make it available on a local server

        bundle exec jekyll serve

5. Browse to [http://localhost:4000](http://localhost:4000)

### 📝 Adding content to the site

#### 📅 Events

1. Clone the project and make a new branch `event/event-name`

1. Make a copy of the [event template](./templates/event-template.md) and place it in the [events directory](./events). Make sure to name it following this pattern `<event-name>-<event-date-YY-mm-dd>`.

1. Fill in the event metadata:

```yml
---
title: Your event name
excerpt: >-
  Text to be displayed in the preview. Make it catchy and descriptive
# note this is the date for the event, not when the post is published
date: '2020-10-15'
# add images to images/events and update the path here. You can use the same image for the thumb and the main image on the post
thumb_image: images/hacktoberfest-folks.jpg
image: images/hacktoberfest-folks.jpg
# Uncomment this if you have registration open, for example, or if you have a call to action
# actions:
#   text: Registration for attendees is now open!
#   url: https://github.com
#   action: Register
#   background: accent
# do not modify the layout
layout: event
---
```

   :warning: Place any images in the [./images/events](./images/events) directory to keep things tidy.

   We have added an `actions` label which can be used to add calls for action such as registration and the such. Uncomment the section and fill in the details:

- **Text**: call for action Text
- **URL**: which URL should folks be redirected to (e.g. Eventbrite, Pretix)
- **action**: the text for the action button
- **background**: any of the background styles (see [Style guide](#style-guide) and [Section colours](#-section-colours) for an example image)

Using the template ensures your event is added to the Events section and sorted by date.

Once completed:

1. Save and commit your changes
2. Push your changes and create a pull request

#### :pencil: Website section

To add a new section to the main page.

1. Clone the project and make a new branch `content/<whatever>`
2. Open [.index.md](./index.md)
3. Add your section where needed:

```yml
- section_id: upcoming_events
 type: section_features
 background: white
 title: Upcoming Events
 subtitle: >-
   Find when the next mentored sprints event is
 features:
   - title: Hacktoberfest 2020
     image: images/wocintech1.jpg
     content: >-
       Let's celebrate Hacktoberfest together! Join folks from Kedro, Terminus DB and Rasa.
     actions:
       - label: Learn More
         url: /events
         primary: true
```

- **section_id**: make sure this is unique to the section
- **background**: see [style guide](#style-guide)
- **actions**: similar to events, this adds a call to action, make sure the URL exists e.g. if redirecting to a new page in the site, there has to be a corresponding `.md` file.

Once completed:

1. Save and commit your changes
2. Push your changes and create a pull request

### :book: Style-guide

#### :art: Colours

The colours used in the site derive from the Mentored Sprints brand colours, but we optimised for web and accessibility:

| Name - theme reference   | COLOUR HEX CODE                                                      |
| ------------------------ | -------------------------------------------------------------------- |
| Light Wisteria - primary        | ![#ce89ce](https://placehold.it/15/ce89ce/000000?text=%20) `#ce89ce` |
| Slate blue -secondary    | ![#4c54c9](https://placehold.it/15/5B63CE/000000?text=%20) `#5B63CE` |
| Midle Blue Green -accent | ![#8DDDD2](https://placehold.it/15/8DDDD2/000000?text=%20) `#8DDDD2` |
| Raisin black - dark      | ![#1B212F](https://placehold.it/15/1B212F/000000?text=%20) `#1B212F` |
| Ghost white - white      | ![#F8F9FF](https://placehold.it/15/F8F9FF/000000?text=%20) `#F8F9FF` |

#### :bookmark: Section colours

The sections in the website can take any of the website colours: `dark`, `accent`, `primary`, `secondary`, or `white`.

For events, these are specified in the YAML header:

```yaml
actions:
  text: Registration for attendees is now open!
  url: https://github.com
  action: Register
  background: accent
```

and are rendered as:

![call to action block](./images/cta.png)

## :raised_hands: Contributing

🚧 This repository is always a work in progress. And everyone is encouraged to help us build something useful to the many. 🚧

Everyone should follow our [Code of Conduct](https://mentored-sprints.netlify.app/code-conduct/) and check out our [Contributing Guidelines](./CONTRIBUTING.md) for more information on how to get started.

## :book: License

The code for this site is Licensed as [BSD-3](https://opensource.org/licenses/BSD-3-Clause) and the content is licensed as
[CC-BY 4.0](http://creativecommons.org/licenses/by/4.0/) ⓒ[Mentored Sprints](https://mentored-sprints.dev).
