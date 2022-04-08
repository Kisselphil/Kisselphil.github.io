# VPRL Website

This site is built with the [Jekyll](https://jekyllrb.com/docs/) static site generator, using the [TeXt](https://github.com/kitian616/jekyll-TeXt-theme) theme. More info can be found at both of those links.

You can find the live version at this url : https://awesome-raman-4b7cb2.netlify.app

## Development

To get started:

- Install [NodeJS](https://nodejs.org/en/download/)
- Install Jekyll
- Run `npm ci` to install dependencies
- Run `npm run serve` to start a dev server. 

## CMS Usage

You can access the Content Management System (CMS) by adding '/admin' to the end of you URL. 

`
https://URL-GOES-HERE/admin
`

Currently accesible via https://awesome-raman-4b7cb2.netlify.app/admin


Once logged in, you should see the sites collections and media.

![Netllify CMS admin page](/assets/readme-docs/netlify-cms.png)

### Edit  Content

For the VPRL Site here is a compelte list of the editable items via the CMS.

- Home Page
- Blog entries 
- People in the Space entries
- Resources Page
- Partners Page
- Navigation Bar

#### Navigation Bar

Found in CMS Collection 'Pages' -> Navigation Bar

You can change the name and the page that a navigation bar option will launch when selected. 
 

**Title**
- The name of the page to appear on the navigation bar

**URL**
- The path to the file where content to be displayed is stored

All URL fields are paths to a file within then the main folder.

#### Home Page

Found in CMS Collection 'Pages' -> 'Home Page'

To replace the images on the Home page, you must replace the following images with an image file with the exact same name. This is because the website references these exact names when building.

- home_card_1.png
- home_card_2.png
- home_card_3.png 


##### Images

To replace the main image on the Home page, you must replace the 'site_home_header.png' image with an image file with the exact same name. This is because the website references this exact name when building.

To replace the card images on the Home page, you must replace the following images with an image file with the exact same name. This is because the website references these exact names when building.

- home_card_1.png
- home_card_2.png
- home_card_3.png 

##### Text Content

Contains the following editable items:
- Title
- Body


##### Card Content

Within the Body of the Home Page there is a large codeblock, this is where the Github, Sidequest, and OSF informtion and links will go. This is one of the HTML elements that I could not add to the CMS but example below should make editing easy.

The code block will consist of 3 HTML elements that look as follows:

```html
<!-- URL to webite goes inside the "" -->
<a href="">
  <div class="card card--clickable">
    <div class="card__image">
      <img class="image" src="/assets/main_github.png"/>
    </div>
    <div class="card__content">
      <div class="card__header">
        <!-- Name of resource goes inside the <h4> tags-->
        <h4>Photograph</h4>
      </div>
      <!-- Description goes inside the <p> tags -->
      <p>...</p>
    </div>
  </div>
</a>
```

#### Blog Entries 

Found in CMS Collection 'Blog'

Every item within the collection is a new blog post on your website. You have the ability to modify previous uploads or create a new blog post.

Each blog will have the following items:
- Title
- Date
- Body

#### People in the Space entries

Found in CMS Collection 'People in the Space'

Every item within this collection is a new item on the People in the Space page. 

Each item requires:
- Name
- Image
- Body
  - Information put here will populate the person's individual page on the website

#### Resources Page

Found in CMS Collection 'Pages' -> 'Resources Page'

##### Slider Images

Images for the Resources page are stored in the media folder.

To replace the images on the Resources page, you must replace the following images with an image file with the exact same name. This is because the website references these exact names when building.

- resources_slider_1.png
- resources_slider_2.png
- resources_slider_3.png
- resources_slider_4.png

##### Text Content

Contains the following editable items:
- Title
- Body



##### Youtube Videos
  - If you wish to add a youtube video, copy/paste this and replace the id 
  ```html
  <div class="embed-container">{%- include extensions/youtube.html id='MoGW3ySNRqg' -%}</div>
  ```


#### Partners Page

Found in CMS Collection 'Pages' -> 'Partners Page'

Contains a list of the following editable items:
- Name
- Bio
- Image

### Change domain

https://docs.netlify.com/domains-https/custom-domains/

### Resources

https://www.markdownguide.org/basic-syntax/
