# Portfolio Site [brandont.dev](https://brandont.dev)

This is the public repo for my portfolio website, currently undergoing an entire redesign. The website will be structured with minimal, light-weight deployment and design principles, getting inspiration from [blot.im](https://blot.im), where I currently run [my blog](https://brandont.blog). 

The site will be developed in Python, using [Django](https://www.djangoproject.com/) (again), however I will not be using Bootstrap or any other frameworks. I may start to dip my toes into some light JavaScript for simple animations and design elements, however I plan on keeping this as simple as possible in every aspect. Light-weight, fast, and easy to update are the themes I'm going with here, and JS may be counter-intuitive to that. I think as long as we keep it very sparse, it would probably be ok, though.

## Roadmap

- Implement a simple git deployment system that will utilize pushing to remote `origin` repositories for backups/version control, and also a bare remote `production` repository that will use hooks to execute `git pull` from a third repository located on the remote VPS. Maybe in the future, we can also Implement a `staging` remote for a staging environment. This change would be simple, but I'm unsure what would be the best long-term method would be for Implementing the environment. 

- Design the `/home` page for the site. The new homepage will have snippets of the most recent blog posts from [brandont.blog](https://brandont.blog), an edited and stylized picture of me (:D), a snippet of my most recent project, and possibly some of my most recent social media posts from [Fosstodon](https://Fosstodon.org/@brandont) and [PixelFed](https://pixelfed.social/bdont). It's possible once I get my stream up and running at another new domain ([brandont.live](https://brandont.live)), I'll also have some kind of embedded video of the stream, or highlights or something.

- Design the `/contact` page for the site. This will be more-or-less almost exactly the same as the previous one, however there will be a reCaptcha implemented (spam is really getting bad), and my social links and email contact info will also be available.

- Design the `/portfolio` page of the site. This will be a bit more complicated than the previous site's `/projects` page. There will be a blog-like "timeline" structure for the projects, however each project will also have its own page, which will contain a more comprehensive breakdown/explination of the details of the project and the development process. I also want to include a Tag system for the projects, and a simple Search function.

- Once each of the site's HTML pages have been flushed out, and the CSS finished, we'll begin working in Django to build out the mechanics of each of the above features. The backend will use SQLite3 to start off; in the future, if a more comprehensive database framework is needed, we'll go with PostgresSQL, but I doubt we'd need something like that with what is currently planned.
