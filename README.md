# Bible For Me

## Purpose

This website is intended to serve as a landing page for people who have received printed gospel tracts and have visited the website on the back. The homepage is intended to be the initial landing page for visitors, and the links on the page go to other pages that give them more information. From the homepage the visitor can view the books offered, and then may select select one. Clicking the link to select a book takes them to the request page, which prompts them to complete the form to request the book.

## Features

* Easy to customize styles via SASS variables
* Easy to add more books to give away
  * Just add a new page with a description of the book and a thumbnail and background image
  * Homepage and request form will update automatically based on the book pages
* Plug in your own contact forms
  * HTML forms for [FormTools](https://formtools.org/) have been added, but they are plain HTML forms that can be wired up to any form service.

## Pages

#### Book Pages

For every book offered on the website there is a book page with a layout of type `book`. Any book page created will show up on the homepage and the request form automatically.

#### About

The about page is a simple markdown page for displaying information on those running the website.

#### Contact

A page displaying a simple contact form with a message box, intended for visitors who have general questions on the site. The form action should be updated to point to the URL of the form service you are using.

#### Contact Confirmation Page

This page shows a confirmation message to the user informing them there contact submission from the contact page has been received. This page should be displayed to the user after they have successfully submitted the contact form. You will need to configure your form service to redirect successful submissions to this page.

#### Request

A page displaying the book request form, intended for visitors would like to receive a printed book by mail. The form requires an email, a street address, and a book title. The form action should be updated to point to the URL of the form service you are using.

#### Request Confirmation Page

This page shows a confirmation message to the user informing them there book request submission from the request page has been received. This page should be displayed to the user after they have successfully submitted the book request form. You will need to configure your form service to redirect successful submissions to this page.

## Forms

Form Tools is used for the forms on the website. You'll need to config them to work with you FormTools instance by adding this markup inside the form tags:

```html
<input type="hidden" name="form_tools_initialize_form" value="1" />
```

## Graphics

Source graphics are stored in `image_sources/`. The final images are stored in `images/`.

### Image Dimensions

Book header graphics

600px x 400px

Book thumbnails

220px x 340px


### Image Credits

<a style="background-color:black;color:white;text-decoration:none;padding:4px 6px;font-family:-apple-system, BlinkMacSystemFont, &quot;San Francisco&quot;, &quot;Helvetica Neue&quot;, Helvetica, Ubuntu, Roboto, Noto, &quot;Segoe UI&quot;, Arial, sans-serif;font-size:12px;font-weight:bold;line-height:1.2;display:inline-block;border-radius:3px" href="https://unsplash.com/@jasonhk1920?utm_medium=referral&amp;utm_campaign=photographer-credit&amp;utm_content=creditBadge" target="_blank" rel="noopener noreferrer" title="Download free do whatever you want high-resolution photos from Jason Wong"><span style="display:inline-block;padding:2px 3px"><svg xmlns="http://www.w3.org/2000/svg" style="height:12px;width:auto;position:relative;vertical-align:middle;top:-2px;fill:white" viewBox="0 0 32 32"><title>unsplash-logo</title><path d="M10 9V0h12v9H10zm12 5h10v18H0V14h10v9h12v-9z"></path></svg></span><span style="display:inline-block;padding:2px 3px">Jason Wong</span></a>

<a style="background-color:black;color:white;text-decoration:none;padding:4px 6px;font-family:-apple-system, BlinkMacSystemFont, &quot;San Francisco&quot;, &quot;Helvetica Neue&quot;, Helvetica, Ubuntu, Roboto, Noto, &quot;Segoe UI&quot;, Arial, sans-serif;font-size:12px;font-weight:bold;line-height:1.2;display:inline-block;border-radius:3px" href="https://unsplash.com/@chuttersnap?utm_medium=referral&amp;utm_campaign=photographer-credit&amp;utm_content=creditBadge" target="_blank" rel="noopener noreferrer" title="Download free do whatever you want high-resolution photos from chuttersnap"><span style="display:inline-block;padding:2px 3px"><svg xmlns="http://www.w3.org/2000/svg" style="height:12px;width:auto;position:relative;vertical-align:middle;top:-2px;fill:white" viewBox="0 0 32 32"><title>unsplash-logo</title><path d="M10 9V0h12v9H10zm12 5h10v18H0V14h10v9h12v-9z"></path></svg></span><span style="display:inline-block;padding:2px 3px">chuttersnap</span></a>

## Similar Websites

* https://chatnow.org/

## Graphics

* https://publicdomainvectors.org/en/free-clipart/Silhouette-vector-drawing-of-old-man-standing/18335.html
* https://publicdomainvectors.org/en/free-clipart/Christ-on-the-cross-vector-image/4215.html

## License

* Code is released under the [MIT License](LICENSE)
* Page content is released under the [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode)

Book covers graphics in this repository are copyright by the respective copyright holders are not released under the MIT license.
