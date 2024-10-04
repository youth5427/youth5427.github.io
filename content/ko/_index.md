---
# Leave the homepage title empty to use the site title
title: 메인페이지
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
        - title: '<span style="font-size:70%">모바일 개발</span>'
          content: '<span style="font-size:70%">모바일 프로젝트를 만나보세요!</span>'
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
            url: /mobiledev
          # 출처: https://unsplash.com/ko/%EC%82%AC%EC%A7%84/space-gray-iphone-x-9e9PD9blAto

        - title: '<span style="font-size:70%">웹 개발</span>'
          content: '<span style="font-size:70%">웹 프로젝트를 만나보세요!</span>'
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
            url: /webdev
          # 출처: https://unsplash.com/ko/%EC%82%AC%EC%A7%84/%EB%A1%9C%EA%B3%A0-JySoEnr-eOg

        - title: '<span style="font-size:70%">기타</span>'
          content: '<span style="font-size:70%">기타 프로젝트를 만나보세요!</span>'
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
            url: /etc
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
      title: '<h1 style="font-size:38px">모바일 개발</h1>'
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
      title: '<h1 style="font-size:38px">웹 개발</h1>'
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
      title: '<h1 style="font-size:38px">기타 프로젝트</h1>'
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
---
