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
  - block: markdown
    id: cv
    content:
      title: CV
      text: You can download my CV here <a href='/uploads/CV_AlfredoAlvarado.pdf'> CV_AlfredoAlvarado </a>
    design:
      columns: '2'
      view: list
  - block: collection
    id: publications
    content:
      title: Recent Publications
      subtitle: <a href='/publication/'>See all publications</a>
      text: 
      count: 3
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: markdown
    id: media
    content:
      title: Recent Media
      subtitle: <a href='/media/'>See all media appearances</a>
      text: <ul><li><a href='https://andina.pe/agencia/noticia-sunafil-estrategia-disminuye-incumplimiento-los-derechos-laborales-915898.aspx'> Sunafil estrategia disminuye el incumplimiento de los derechos laborales</a>.</li> <li><a href='http://blog.pucp.edu.pe/blog/idhal/2021/02/09/el-rompecabezas-de-la-informalidad/'> El rompecabezas de la informalidad</a>.</li> <li><a href='https://departamento.pucp.edu.pe/economia/charlas-y-conferencias/viernes-economico-empleo-e-ingresos-laborales-peru/'> Viernes Económico Empleo e Ingresos Laborales en el Perú</a>.</li></ul>
      filters:
        folders:
          - media
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: list
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
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
