# mentored-sprints.dev
<div align="center">
 <img alt="Logo" src="https://github.com/pycon-mentored-sprints/digital-assets/blob/master/logos/blue-pink-text.svg?raw=true" width="250" />
</div>
<br>

[![License](https://img.shields.io/badge/License-BSD%203--Clause-gray.svg?colorA=2D2A56&colorB=7A76C2&style=flat.svg)](https://opensource.org/licenses/BSD-3-Clause)

- [mentored-sprints.dev](#mentored-sprintsdev)
  - [💻 Development](#-development)
    - [Running this Site Locally](#running-this-site-locally)
    - [📝 Adding content to the site](#-adding-content-to-the-site)
      - [📅 Events:](#-events)
  - [Contributing](#contributing)
  - [License](#license)

This reposiroty contains the source code for [mentored-sprints.dev](mentored-sprints.dev which is the main website for the project, events and the such. If you are looking for the source for the [Community Handbook](https://github.com/pycon-mentored-sprints/community-handbook) head to [https://github.com/pycon-mentored-sprints/community-handbook](https://github.com/pycon-mentored-sprints/community-handbook).

## 💻 Development

### Running this Site Locally

This website is build using Jekyll and served through Netlify. If you want to make changes to the site follow these steps to work on this on your local computer.

1. Install a full [Ruby development environment](https://jekyllrb.com/docs/installation/)

2. Install Jekyll and Bundler

        gem install jekyll bundler

3. Install dependencies from Gemfile:

        bundle install
4. Build the site and make it available on a local server

        bundle exec jekyll serve

5. Browse to [http://localhost:4000](http://localhost:4000)

### 📝 Adding content to the site

#### 📅 Events:

1. Clone the project and make a new branch `event/event-name`

1. Make a copy of the [event template](./templates/event-template.md) and place it in the [events directory](./events). Make sure to name it following this pattern `<event-name>-<event-date-YY-mm-dd>`.

3. Fill in the event metadata:
```yml
---
title: Your event name
excerpt: >-
  Text to be displayed in the preview. Make it catchy and descriptive
# note this is the date for the event not when the post is published
date: '2020-10-15'
# add images to images/events and update the path here, you can use the same image for the thumb and the main image on the post
thumb_image: images/hacktoberfest-folks.jpg
image: images/hacktoberfest-folks.jpg
# Uncomment this is you have registration open for example, or if you have a call to action
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
   - **url**: which URL should folks be redirected to (e.g. Eventbrite, pretix)
   - **action**: the text for the action button
   - **background**: any of the background styles (see [Style guide](#style-guide))

This will automatically add your event to the Events page and sort by date.

1. Save and commit your changes
1. Push your changes and create a pull request

### Style-guide


## Contributing

🚧 This repository is always a work in progress and everyone is encouraged to help us build something that is useful to the many. 🚧

Everyone is asked to follow our [Code of Conduct](https://www.mentored-sprints.dev/code-conduct/) and to checkout our [Contributing Guidelines](./CONTRIBUTING.md) for more information on how to get started.

## License

The code for this site is Licensed as [BSD-3](https://opensource.org/licenses/BSD-3-Clause) and the content is licensed as
[CC-BY 4.0](http://creativecommons.org/licenses/by/4.0/) ⓒ[Mentored Sprints](mentored-sprints.dev)