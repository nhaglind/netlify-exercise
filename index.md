---
layout: default
---

<p class="question">Rank your 5 favorite, and least favorite, activities from this <a href="https://gist.github.com/fool/b0f254ff8c72a5765b6a9138249789d6">list</a>:</p>

<p>Most Favorite</p>
<ul>
  <li>Work with the development team to help design a new feature based on feedback from customers</li>
  <li>Work with people to figure out if Netlify's service can solve a particular workflow or integration challenge they have</li>
  <li>Set up your own copy of several static site frameworks for debugging</li>
  <li>Help train and onboard new support teammates</li>
  <li>Create video tutorials to help teach users a specific feature or use case</li>
</ul>
<p>Least Favorite</p>
<ul>
  <li>Dig through server logs to troubleshoot a customer's website behavior</li>
  <li>Analyze thousands of support tickets to spot trends to improve our product</li>
  <li>Submit bug reports and potentially bug fixes to closed and open source projects that Netlify maintains on GitHub</li>
  <li>Debug a customer's build using a programming language and framework that you've never seen before</li>
  <li>Help manage communications during a service outage</li>
</ul>

<p class="question">What is your favorite thing about providing technical support?</p>
<p>The immediate feedback loop, it's quite gratifying to have problems that right away provide a result. Working through a difficult problem and experiencing the excited reaction of the person you helped is incredible. What might have been small to you, could have been huge for the user whether it saved them time, money, etc.</p>

<p class="question">What did you think of our service during the time you used it?  Be honest!  “it sucked” isn’t a wrong answer unless you don’t elaborate and provide some constructive criticism ;)</p>
<p>It almost worked "too well", I tweeted Tim about this. I flipped my personal site over to Netlify and what was typically a cumbersome task like forcing HTTPS in htaccess or setting up SSL (getting this to work on our rails site with Let's Encrypt at the time required way too many do-overs because of tiny typos) was done with a push of a button. <em>Magic!</em></p> 

<p>A common issue that many businesses face and why they can be steered to choose a CMS is because of form handling and how they process intake. The site may have different forms on each page, each one needs to pass variables to send emails a certain way, and if there was a graceful way to do this (perhaps capture the submission statistics similar to how mailgun approaches this) there might be an opportunity to improve in this space.</p>

<p class="question">Tell about how you made your site and why you chose the tools you did.  Briefly explain a challenge you experienced in setting up this site and how you solved it.</p>
<p>I think Jekyll is pretty slick and since I'm familiar using it, Jekyll made the most sense which allowed more time devoted to answering questions. I also wanted to keep the Netlify aesthetic going so I used Chrome DevTools to extract the pretty colors! Ran some simple commands to create the files and then added the project to a local git repo and pushed to Github followed by the easy deploy to Netlify.</p>

<p>The biggest challenge was setting up the redirect. Luckily, it was fast to find the documentation located <a href="https://www.netlify.com/docs/redirects/">here</a>. I must admit I was unsure if I needed to put it in a special folder or add an extension to the file as <code>_redirects</code> looked similar to the convention for folders e.g. _includes or _layouts that Jekyll uses.</p>

<p class="question">Could you give us a suggestion to improve this test or the job posting?</p>
<p>It would be helpful to have an overview or a link to a blog post in the job listing explaining a "day in the life as a <u>support engineer</u>." I know for many jobs and likely this one as well, the workday can vary greatly, but it might be nice to see what a typical schedule would look like. </p>

<p class="question">Provide a link to documentation for a technical/developer-focused product, that you think are well done, and briefly explain why you think they are well done.</p>

<p>Personally, I find the <a href="https://stripe.com/docs">Stripe</a> documentation beautiful. The smooth transitions between languages, examples for testing, the little pop-ups in the code snippets (pictured below), the positioning of search at the top but within the container with auto-complete, and the logical structure in the nav.</p> 

<p>Handling payments is frightening for a developer, but Stripe gave their docs some serious TLC to calm that fear which was a great decision.</p>

<img src="/assets/images/stripe-doc.png" width="100%"> 

<p class="question">Why do you think SSL/HTTPS is important?</p>

<p>The potential for man-in-the-middle attacks or how often we'll encounter spoof sites, makes it almost necessary as we continue to increase our reliance on web applications for all aspects in life whether that's banking, shopping, relationships, etc. We must do everything we can to gain trust from our users and reduce the burden on everyone having to be an IT security expert to simply browse the web safely.</p>

<p>Before Let's Encrypt, the costs and difficulty of signing, validating, and installing was prohibitive to small businesses that didn't have the resources. Thankfully, such efforts exist and the trend of secure sites is <a href="https://letsencrypt.org/stats/#growth">sharply rising</a>.</p>

<p class="question">Explain, in a couple of paragraphs, what you think 2 major challenges around DNS configuration are for less-technical internet end-users</p>

<p>Honestly, the fear of being down and doing it in the first place. You're changing your address and when you do this, things can break, you <em>may</em> be down for however long. The change to Netlify took about 2 minutes but I've seen others take quite a bit longer to propagate.</p>

<p>Finding the right name servers to use and waiting to see if it's even right is often troublesome especially if the documentation is poor. If you need to do some other advanced DNS items like pointing to email providers, adding additional CNAME records, specifying TTL, and other non-obvious items add overhead to the user.</p>

<p class="question">A customer writes in saying their “site won’t build”.  Compose your best short (2-paragraph) customer-facing answer without any additional data, that could be useful in the generic case but would also lead to a customer providing a more actionable response.</p>

<p>Hey user, I’m sorry to hear that you’re having trouble with the build but I’m sure we can work together to figure this out! Our most common reasons for an unsuccessful build are x, y, and z.</p> 

<p>Here are some guides that specifically address those difficulties. If none of those seem to help, I’d be more than happy to delve deeper into what might be going on here but I’ll need a little bit more background information on what you’ve previously tried and with what’s happening.</p>
