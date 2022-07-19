# Portfolio Site [brandont.dev](https://brandont.dev)

This is the public repo for my portfolio website, currently undergoing an entire redesign. The website will be structured with minimal, light-weight deployment and design principles, getting inspiration from [blot.im](https://blot.im), where I currently run [my blog](https://brandont.blog). 

The site will be developed in Python, using [Django](https://www.djangoproject.com/) (again), however I will not be using Bootstrap or any other CSS and style frameworks like the last site. I may start to dip my toes into some light JavaScript for simple animations and design elements, however I plan on keeping this as minimalist as possible in every aspect. Light-weight, fast, and easy to update are the themes I'm going with here, and JS may be counter-intuitive to that (I also realize that Python may also be counter to this, but there are some consessions I'm willing to make here). I think as long as we keep it very sparse, it would probably be ok, though.

## Roadmap
The order in which I complete these items are subject to change, given any unexpected issues we may find along the development process, or any changes of heart I may have. However, I'd like to first tackle a robust development and deployment setup using just git, as explained below. 

- Implement a simple git deployment system that will utilize pushing to remote `origin` repositories for backups/version control, and also a bare remote `production` repository that will use hooks to execute `git pull` from a third repository located on the remote VPS. Maybe in the future, we can also Implement a `staging` remote for a staging environment. This change would be simple, but I'm unsure what would be the best long-term method for Implementing the staging environment. 

- Create dynamic `settings.py` files for both development and production environments. We want to make deployment as simple as possible, and keep the development and deployment environments segmented in an intuitive way. 

- Build the backend mechanics for the more complex pages. This will mostly just be the `/portfolio` page itself and the individual `/project` page, where each project in the portfolio will have its own blog-style page, but some of the elements of the `/home` page will also need to be sused out in this step.

- `/home` The new homepage will have snippets of the most recent blog posts from [brandont.blog](https://brandont.blog), an edited and stylized picture of me (:D), a snippet of my most recent project, and possibly some of my most recent social media posts from [Fosstodon](https://Fosstodon.org/@brandont) and [PixelFed](https://pixelfed.social/bdont). It's possible once I get my stream up and running at another new domain ([brandont.live](https://brandont.live)), I'll also have some kind of embedded video of the stream, or highlights or something.

- `/contact` The contact page will be more-or-less almost exactly the same as the previous one, however there will be a reCaptcha implemented (spam is really getting bad), and my social links and email contact info will also be available.

- `/portfolio` This will be a bit more complicated than the previous site's `/projects` page. There will be a blog-like "timeline" structure for the projects, however each project will also have its own page, which will contain a more comprehensive breakdown/explination of the details of the project and the development process. I also want to include a Tag system for the projects, and a simple Search function.
