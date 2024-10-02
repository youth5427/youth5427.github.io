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
        - title: '<span style="font-size:70%">네이버</span>'
          content: '<span style="font-size:70%">네이버테스트</span>'
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
            url: "https://naver.com"

        - title: '<span style="font-size:70%">다음</span>'
          content: '<span style="font-size:70%">다음테스트</span>'
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
    design:
      view: compact
      columns: "2"

  - block: collection
    content:
      id: section-1
      title: 기타 프로젝트
      count: 2
      offset: 0
      order: desc
      filters:
        folders:
          - etc
    design:
      view: compact
      columns: "2"
  - block: project
    content:
      # # Page type to display. E.g. project.
      page_type: project

      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      filter_default: 0

      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      filter_button:
        - name: 전체
          tag: "*"
        - name: 모바일 개발
          tag: MD
        - name: 웹 개발
          tag: WD
        - name: 기타
          tag: etc

    design:
      columns: "1"
      view: masonry
      flip_alt_rows: true
      background: {}
      spacing: { padding: [0, 0, 0, 0] }
---
