---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
     username: admin
  - block: collection
    id: publications
    content:
      title: Recent Publications
	  subtitle: <a href='/publication/'>See all publications</a>
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      count: 3
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: markdown
    id: media
    content:
      title: Recent media
	  subtitle: <a href='/media/'>See all media appearances</a>
      text: 
      filters:
        folders:
          - media
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: list
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      email: alvarado.a@pucp.pe
      address:
        city: Washington
        region: DC
        country: United States
        country_code: US
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/alfredoman'
      # Automatically link email and phone or display as text?
      autolink: true
    design:
      columns: '2'
---
