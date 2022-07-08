# Brandon's Portfolio Site [brandont.dev](https://brandont.dev)

This is the public repo for my portfolio website, current undergoing an entire redesign. The website will be structured with minimal, light-weight deployment and design principles, getting inspiration from [blot.im](https://blot.im), where I currently run [my blog](https://brandont.blog). 

The site will be developed in [Django](https://www.djangoproject.com/) (again), however I will not be using Bootstrap or any other frameworks. I may start to dip my toes into some light JavaScript for some simple animations and design elements, however I plan on keeping this a simple as possible in every aspect. Light-weight, fast, and easy to update are the themes I'm going with here.

## Roadmap

- [] Implement a simple git deployment system that will utilize pushing to both remote `origin` repositories, and also a bare `production` repository that will use hooks to execute `git pull` from a third production repository located on the remote VPS.

- [] Design the `/home` page for the site. The new homepage will have snippets of the most recent blog posts from [brandont.blot](https://brandont.blog), an edited and stylized picture of me (:D), a snippet of my most recent project, and possibly some of my most recent social media posts from Fosstodon and PixelFed. It's possible once I get my stream up and running at another new domain ([brandont.live](https://brandont.live)), I'll also have some kind of embedded video of the stream, or highlights or something.

- [] Design the `/contact` page for the site. This will more-or-less be almost exactly the same as the previous one, however there will be a reCaptcha implemented as well (spam is really getting bad), and my social links/email contact info will also be available.

- [] Design the `/portfolio` page of the site. This will be a bit more complicated than the previous site's `/projects` page. There will be a blog-like "time-line" structure of the projects, however each project will also have their own page, which will contain a more comprehensive breakdown/explination of the details of the project and the development process. I also want to include a Tag system for the projects, and a simple Search function.
