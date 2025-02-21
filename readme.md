# How to add/edit things on the website
Relevant folders
```
├── assets
│   ├── images
│   │   ├── core_logos  (add new logo of the CORE here)
│   │   ├── organization_logos (add logos of the other organizations here)
│   │   ├── contributors_photos (add photos of contributors here)
├── config
│   ├── _default
│   │   ├── languages.toml (change only if interested in adding a website version in another language)
│   │   ├── menus.en.toml (what's in the top and footer menus)
│   │   ├── module.toml
│   │   ├── params.toml (here you can change stuff like the menu logo, the favicon and other website metadata)
├── content
│   ├── english
│   │   ├── about
│   │   ├── authors
│   │   ├── blog
│   │   ├── contact
│   │   ├── organizations
│   │   ├── pages
│   │   ├── sections
│   │   ├── _index.md
├── data
│   ├── social.json (change here the social media links of the organization)
│   ├── theme.json (change the website theme and colors)
├── themes
│   ├── hugoplate
│   |   ├── layout
│   |   |    ├── index.html (home page layout)
│   |   |    ├── organizations (below applies also to other folders such as "authors")
│   |   |    |    ├── list.html (layout of the list of organization cards on the corresponding page)
│   |   |    |    ├── single.html (layout of each organization's separate page, not used for now)
│   |   |    ├── partials (layout for part of a page, which can be used in other layouts with a `{{ partial ... }}` block)
```

## Add a new organization
1. create an `org-name.md` file in the folder `content/english/organizations`, copying the structure of the ones already there.
2. add logo to the folder `assets/images/organizations_logos`.

## Add a new contributors
1. create an `contrib-name.md` file in the folder `content/english/authors`, copying the 
structure of the ones already there.
2. add your picture in 1:1 aspect ratio to the folder `assets/images/contributors_photos`.

## Add a new calendar event 
1. add the event in Google Calendar, it will automatically appear in the website and posted to Bsky.
