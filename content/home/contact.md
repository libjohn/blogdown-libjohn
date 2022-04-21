---
# An instance of the Contact widget.
# Documentation: https://sourcethemes.com/academic/docs/page-builder/
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 150

title: Contact
subtitle:

content:
  # Automatically link email and phone or display as text?
  autolink: true
  
  # Email form provider (replace nobody with formspree or netlify)
  form:
    provider: netlify
    formspree:
      id: test
    netlify:
      # Enable CAPTCHA challenge to reduce spam?
      captcha: true
  
design:
  columns: '2'
---
