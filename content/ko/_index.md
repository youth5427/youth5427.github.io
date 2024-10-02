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

  - block: slider
    content:
      slides:
        - title: '<span style="font-size:70%">모바일 개발</span>'
          content: '<span style="font-size:70%">모바일 프로젝트를 만나보세요!</span>'
          align: center
          background:
            image:
              filename: ocean.jpg
              filters:
                brightness: 0.4
            position: center
            color: "#000"
          link:
            icon: mobile-alt
            icon_pack: fas
            text: ""
            text-color: "#fff"
            url: /mobiledev

        - title: '<span style="font-size:70%">웹 개발</span>'
          content: '<span style="font-size:70%">웹 프로젝트를 만나보세요!</span>'
          align: center
          background:
            image:
              filename: ocean.jpg
              filters:
                brightness: 0.4
            position: center
            color: "#000"
          link:
            icon: external-link-alt
            icon_pack: fas
            text: "출처"
            text-color: "#fff"
            url: "https://daum.net"

        - title: '<span style="font-size:70%">기타</span>'
          content: '<span style="font-size:70%">기타 프로젝트를 만나보세요!</span>'
          align: center
          background:
            image:
              filename: ocean.jpg
              filters:
                brightness: 0.4
            position: center
            color: "#000"
          link:
            icon: external-link-alt
            icon_pack: fas
            text: "출처"
            text-color: "#fff"
            url: "https://daum.netA"

    design:
      slide_height: "350px"
      slide_width: "100%"
      is_fullscreen: false
      loop: true
      interval: 3000

  - block: collection
    content:
      id: section-1
      title: 모바일 개발
      count: 2
      offset: 0
      order: desc
      filters:
        folders:
          - mobiledev
      sort_by: "date"
      sort_ascending: false
    design:
      view: compact
      columns: "2"

  - block: collection
    content:
      id: section-2
      title: 웹 개발
      count: 2
      offset: 0
      order: desc
      filters:
        folders:
          - webdev
      sort_by: "date"
      sort_ascending: false
    design:
      view: compact
      columns: "2"

  - block: collection
    content:
      id: section-3
      title: 기타 프로젝트
      count: 2
      offset: 0
      order: desc
      filters:
        folders:
          - etc
      sort_by: "date"
      sort_ascending: false
    design:
      view: compact
      columns: "2"
---
