---
# Leave the homepage title empty to use the site title
title:
date: 2024-03-25
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: ""
      username: admin
    design:
      background:
        image:
          filename: background.jpg
          # Optional: Set background image options
          size: cover
          position: center
          parallax: false

  - block: slider
    content:
      slides:
        - title: '<span style="font-size:70%">Mobile</span>'
          content: '<span style="font-size:70%">Meet the Mobile Projects!</span>'
          align: center
          background:
            image:
              filename: mobileslide.jpg
              filters:
                brightness: 0.4
            position: center
            color: "#000"
          link:
            icon: mobile-alt
            icon_pack: fas
            url: /en/mobiledev
          # 출처: https://unsplash.com/ko/%EC%82%AC%EC%A7%84/space-gray-iphone-x-9e9PD9blAto

        - title: '<span style="font-size:70%">Web</span>'
          content: '<span style="font-size:70%">Meet the Web Projects!</span>'
          align: center
          background:
            image:
              filename: webslide.jpg
              filters:
                brightness: 0.4
            position: center
            color: "#000"
          link:
            icon: code
            icon_pack: fas
            url: /en/webdev
          # 출처: https://unsplash.com/ko/%EC%82%AC%EC%A7%84/%EB%A1%9C%EA%B3%A0-JySoEnr-eOg

        - title: '<span style="font-size:70%">Etc</span>'
          content: '<span style="font-size:70%">Meet the etc projects!</span>'
          align: center
          background:
            image:
              filename: etcslide.jpg
              filters:
                brightness: 0.4
            position: center
            color: "#000"
          link:
            icon: laptop-code
            icon_pack: fas
            url: /en/etc
          # 출처: https://unsplash.com/ko/%EC%82%AC%EC%A7%84/macbook-pro-showing-programming-language-xrVDYZRGdw4
    design:
      slide_height: "350px"
      slide_width: "100%"
      is_fullscreen: false
      loop: true
      interval: 3000

  - block: collection
    content:
      id: section-1
      title: '<a href="/en/mobiledev"><h1 style="font-size:38px">Mobile development</h1></a>'
      count: 2
      offset: 0
      order: desc
      filters:
        folders:
          - mobiledev
      sort_by: date
      sort_ascending: false
    design:
      view: compact
      columns: "2"

  - block: collection
    content:
      id: section-2
      title: '<a href="/en/webdev"><h1 style="font-size:38px">Web development</h1></a>'
      count: 2
      offset: 0
      order: desc
      filters:
        folders:
          - webdev
      sort_by: date
      sort_ascending: false
    design:
      view: compact
      columns: "2"

  - block: collection
    content:
      id: section-3
      title: '<a href="/en/etc"><h1 style="font-size:38px">Etc projects</h1></a>'
      count: 2
      offset: 0
      order: desc
      filters:
        folders:
          - etc
      sort_by: date
      sort_ascending: false
    design:
      view: compact
      columns: "2"

  - block: skills
    content:
      title: Development environment
      username: admin
      position: center
---
