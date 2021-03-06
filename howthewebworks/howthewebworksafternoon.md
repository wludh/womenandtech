# How the Web Works, Part 2

![gif of a cat wearing a pink wig typing on a computer](https://media.giphy.com/media/lXiRzPb8C5JTJcfPq/giphy.gif)

Now that we're HTML/CSS experts...

## What belongs in a web site?

![gif of homer simpson's web page, which is all animated toasters and a dancing Jesus](https://media.giphy.com/media/hNAIvVn5ZW3ug/giphy.gif)

Probably fewer gifs than on Homer's page (or in this workshop). Either way, what belongs in a web site depends on the kind of site you're creating. Some types of sites you might want to build include:

### Personal/professional sites

- [6 Things You Should Put on Your Personal Website—and 6 Things to Avoid at All Costs](https://www.themuse.com/advice/6-things-you-should-put-on-your-personal-websiteand-6-things-to-avoid-at-all-costs)
- [The Essential Components Of A Great Personal Website](https://collegeinfogeek.com/essential-components-of-personal-websites/)
- [Why Every Job Seeker Should Have a Personal Website, And What It Should Include](https://www.forbes.com/sites/jacquelynsmith/2013/04/26/why-every-job-seeker-should-have-a-personal-website-and-what-it-should-include/#2dbfa5e9119e)
- [What Should I Include On My Personal Website? These 7 Things Will Make Sure Your Website Stands Out](https://www.bustle.com/p/what-should-i-include-on-my-personal-website-these-7-things-will-make-sure-your-website-stands-out-2803041)

### Blogs

- [7 Simple Ways Blogging Can Benefit Your Career](https://www.thebalancecareers.com/ways-blogging-can-benefit-your-career-4044842)
- [How to start a blog: 11 pro tips](https://www.creativebloq.com/web-design/how-to-start-a-blog-1131726)

### Art or photography portfolios

- [The Dos And Don’ts Of Building A Photography Portfolio](https://www.shawacademy.com/blog/dos-and-donts-of-building-a-photography-portfolio/)
- [Create a Professional Photography Portfolio in 5 Steps](https://expertphotography.com/create-a-photography-portfolio/)
- [6 Steps To Creating A Knockout Online Portfolio](https://99u.adobe.com/articles/7127/6-steps-to-creating-a-knockout-online-portfolio)
- [Building the Best Online Portfolio for Your Art](https://www.artworkarchive.com/blog/building-the-best-online-portfolio-for-your-art)

## How do you decide what the design of your site should be?

![gif of Joey from Friends saying, "When the package is this pretty, no one cares what's inside"](https://media.giphy.com/media/ubQOPZPbPPJ7y/giphy.gif)

We usually know good design when we see it, but it can be harder to produce it ourselves. It helps to review some tips for effective web design:

- [10 Top Principles of Effective Web Design](https://shortiedesigns.com/2014/03/10-top-principles-effective-web-design/)
- [4 key principles of web design](https://99designs.com/blog/tips/web-design-basics-guide/)
- [6 principles of visual hierarchy for designers](https://99designs.com/blog/tips/6-principles-of-visual-hierarchy/)
- [12 Visual Hierarchy Principles Every Non-Designer Needs to Know](https://visme.co/blog/visual-hierarchy/)

But one of the most important parts of good design is to suit the design to the content, uses, and audience. This means good design will vary depending on what your goals are for your website. For that reason, it can be helpful to start by thinking about what your website needs to do, and how it should look in order to accomplish that.

### Sketching and wireframing

Before you start building your website--even before you start looking at themes and templates--it helps to get your design ideas organized. Start with a rough sketch of the page. Where will the images go? Where will the menu go? Which content will go on which part of the page, and in what order?

Once you have a sketch, you can move on to a wireframe, which is a more complete plan of your website design and organization. You can make a wireframe using paper and pencil, or using one of several digital tools for wireframing.

- [Planning Your Web Design with Sketches](https://tympanus.net/codrops/2013/01/29/planning-your-web-design-with-sketches/)
- [How to make your first wireframe](https://www.invisionapp.com/inside-design/how-to-wireframe/)
- [The Definitive Guide: How To Create Your First Wireframe](https://careerfoundry.com/en/blog/ux-design/how-to-create-your-first-wireframe/)
- [How to Design a Useful Wireframe](https://blog.teamtreehouse.com/how-to-design-a-useful-wireframe)

## Publishing your website 
You've been viewing your website in your browser, but it's not yet live on the Web. To do so, we need to upload the files to the server that hosts your website. Remember, a website is just a collection of files and folders on someone's computer. Let's take a quick tour through the hosting environment of your new website. 

### Reclaim Hosting
Your website (username.wludci.info) is hosted by a company called [Reclaim Hosting](http://www.reclaimhosting.com). They provide web hosting for individuals and educational organizations like W&L. While there are lots of web hosting companies out there, we like Reclaim because of their educational focus and excellent support. 

For more help:
* [Reclaim Support](https://community.reclaimhosting.com/)
* [Davidson/Emory Documentation](http://domains.davidson.edu/support/getting_started/getting_started)

Back up, what does a web hosting company even do? In our case, Reclaim registers the domain name so when someone visits it, it brings them to the right content. They provide storage space for your text, images, video, and other content. They provide applications that help you install and run WordPress and many other content management systems. You can even set up your own email through your domain. 

### CPanel
Most of the stuff you do with your domain happens in the Control Panel or Cpanel. You can access the CPanel by adding `/cpanel` to the end of your domain name. Log in with the username and password provided in an email, and you should see a whole dashboard of icons. From here, you can upload files, install applications, or change any settings. 

### Okay let's make it live! 
To make your HTML and CSS live on the web, you'll need to upload the files to your website. 

1. Start in CPanel.
2. Click on File Manager. A new tab should open with a list of files and folders. These are all the things on your domain! 
3. If you're not already there, navigate to `public_html`. This is where you'll put anything that should be live on the web. 
4. Click on Upload, then drag your HTML and CSS documents to the window. You can also select `Select File` and upload each file individually. 
5. Now visit your website `http://username.wludci.info` and see the results! 

![gif of Constance Wu from Fresh Off the Boat saying, "Success"](https://media.giphy.com/media/26BRCoPeetq9cAdhK/giphy.gif)

### Wait, did you say WordPress? 
WordPress is a commonly used content management system. It powers many of the sites you visit every day. You might have used WordPress for a class project. You can create as many WordPress sites as you want on your website using the Installatron. 

1. From CPanel, click on `WordPress`. 
2. On the right, click on the `install this application` box. 
3. Work through the form, accepting the defaults, EXCEPT... 
4. Pay close attention to the Location options. If you install WordPress to your domain without specifying a directory, it will install at the root of your website, wiping out anything that might be there already. Typing something in the directory field will install WordPress to that directory/folder. 
5. You might want to change the Administrator Username and Password to something you'll remember. 
6. When you're done, click `Install`. 
7. You'll be able to see your WordPress installation in `My Apps` in CPanel. You can use the link that ends with "admin" to login. 

## HTML5 UP themes

You may not need anything as big and complicated (in terms of the code) as WordPress, but you also may not quite be ready to build your own site from the ground up. Fortunately, there's a middle ground. Well, several kinds of middle ground. One is to use a static site generator like [Jekyll](https://jekyllrb.com/) or [Hugo](https://gohugo.io/). Doing that requires a bit of experience with the [command line](https://lifehacker.com/a-command-line-primer-for-beginners-5633909), but it's definitely something you can figure out if you're interested.

Another option is to download an HTML template and modify it to suit your needs. Doing this requires some knowledge of HTML and CSS (which you now have!), but a lot of the work is done for you, letting you experiment and try things out. You can make changes and see how they work out right away by loading the pages on your browser. There are lots of places to find templates, but one good starting place is [HTML5 UP](https://html5up.net/).

## Try it out

- Download a template from HTML5 UP that fits the design you sketched earlier.
- Use your text editor to add some content--maybe just your name and some information, or maybe a picture or two.
- Open the new page in your web browser.

### How's it look?

![gif of a girl in a birthday hat excitedly picking up a glass bowl and throwing it to the ground](https://media.giphy.com/media/yoJC2GnSClbPOkV0eA/giphy.gif)

