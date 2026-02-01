jQuery Handlers & Purpose

This document lists the main jQuery selectors, handlers and where they are defined.

- Main slider initialization: js/main.js
  - Selector: $(".Modern-Slider").slick({...})
  - Purpose: Autoplay hero slides with fade, dots and navigation arrows.

- Mobile nav toggle: js/main.js
  - Selector: $('#nav-toggle').on('click', ...)
  - Purpose: Toggle `#main-nav` open/closed on small screens.

- Tabs behavior: js/main.js
  - Selector: $('.tabs a').click(...)
  - Purpose: Show/hide tab panels in the blog/tabs section.

- Video box autoplay: js/main.js
  - Selector: $(".box-video").click(...)
  - Purpose: Append autoplay parameter to iframe and add open state.

- Owl carousel init: js/main.js
  - Selector: $('.owl-carousel').owlCarousel({...})
  - Purpose: Initialize responsive carousel for services/portfolio items.

- Smooth scrolling & navigation highlight: js/main.js
  - Selectors/Functions: navigation.on('click','a',...), updateNavigation(), smoothScroll(target)
  - Purpose: Smoothly scroll to sections and add/remove `active-section` on nav links based on scroll position.

- Button anchor smooth scroll: js/main.js
  - Selector: $('.button a[href*=#]').on('click', ...)
  - Purpose: Animate page scroll for in-page CTA links.

- Read More modal: index.html
  - Selector: $(document).on('click', '.read-more', ...)
  - Purpose: Load hidden article HTML into `#articleModalBody` and show `#articleModal`.
  - Hidden article content blocks live under `#articles` in index.html.

Notes
- Bootstrap's JS (`js/vendor/bootstrap.js`) is required for modal behavior and depends on jQuery.
- Make sure only one jQuery include is present (index.html uses the v1.11.2 CDN/local fallback).

If you'd like, I can extract each handler into a separate small module or add more comments to other JS files.
