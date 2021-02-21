---
layout: layouts/post.njk
title: Contact
templateClass: tmpl-post
eleventyNavigation:
  key: Contact
  order: 5
---

<figure class="figure">
  <img src="../img/contact.jpg" class="img-fluid" alt="A pen and paper">
  <figcaption class="figure-caption">
Photo by <a href="https://unsplash.com/@aaronburden?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Aaron Burden</a> on <a href="https://unsplash.com/s/photos/contact?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a>  </figcaption>
</figure>


<form name="contact" method="POST" data-netlify="true">
  
  <!-- First name -->
  <div class="mt-4 mb-4">
    <label class="form-label" for="firstname" >First name:</label>
    <input type="text" class="form-control" id="firstname"  name="firstname" placeholder="Enter your first name" required>
  </div>
  
  <!-- Surname -->
  <div class="mt-4 mb-4">
    <label class="form-label" for="surname" >Surname:</label>
    <input type="text" class="form-control" id="surname"  name="surname" placeholder="Enter your surname" required>
  </div>

  <!-- Email address -->
  <div class="mb-4">
    <label class="form-label" for="email">Your email address:</label>
    <input type="email" class="form-control" id="email" name="email" placeholder="Enter your email address" required>
  </div>
  
  <!-- Message -->
  <div class="mb-4">
    <label class="form-label" for="message">Your Message:</label>
    <textarea class="form-control" id="message" name="message" placeholder="Enter your message" required></textarea>
  </div>
  
  <!-- Submit -->
  <button class="btn btn-primary" type="submit">Send</button>

  
</form>