# Horiseon seo-refactor Challenge

Application is live at https://haydennease.github.io/seo-refactor/

## Areas of Focus 
- [Metadata](#metadata)
- [HTML Semantics](#html-semantics)
- [Usability Improvements](#usability-improvements)
- [Bloat Reduction](#bloat-reduction)

## Metadata
The webpage was lacking almost all of its necessary `metadata`. 

`description`, `keywords`, and `viewport` were added to increase search engine optimization and improve display properties.

## HTML Semantics
In an effort to increase the accessability of the webpage, all preexisting `div` tags were replaced with their relative semantic elements of: 
- `header`
- `section`
- `body`
- `article`
- `aside`
- `footer`

These allow a browser to more effectively understand the elements' content and improve accessability for the user.

## Usability Improvements
The focus of these changes was primarily on the `nav` bar. 

![nav bar](/assets/images/nav%20bar.png)
1. When a user moves their curser over *Hori**seo**n*, a  hover feature appears to convey the service's commitment to **S**earch **E**ngine **O**ptimization. 
2. A hover feature was added to the anchor links in order to display an underline - enhancing their visibility.

Additionally, the images contained in the `body` and `aside` were given image `alts` to improve SEO and accessability.

## Bloat Reduction
Almost all of the preexisting class elements for the page were redundant: 
```
.search-engine-optimization {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.online-reputation-management {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.social-media-marketing {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}
```

All of the identical class styles were consolidated into singular semantic elements in both HTML and CSS:  
```
article {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}
```