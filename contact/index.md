---
layout: layouts/post.njk
title: Contact
templateClass: tmpl-post
eleventyNavigation:
  key: Contact
  order: 5
---

<form name="contact" method="POST" data-netlify="true">
  
  <!-- Name -->
  <div class="mt-4 mb-4">
    <label class="form-label" for="name" >Your Name:</label>
    <input type="text" class="form-control" id="name"  name="name" placeholder="Enter your name">
  </div>
  
  <!-- Email -->
  <div class="mb-4">
    <label class="form-label" for="email">Your Email:</label>
    <input type="email" class="form-control" id="email" name="email" placeholder="Enter your email">
  </div>
  
  <!-- Role -->
  <div class="mb-4">
    <label class="form-label" for="role">Your Role:</label>
    <select class="form-select" id="role" name="role[]" multiple>
        <option value="leader">Leader</option>
        <option value="follower">Follower</option>
    </select>
  <div id=roleHelpText class="form-text">
      Choose as many as apply
    </div>
  </div>
  
  <!-- Message -->
  <div class="mb-4">
    <label class="form-label" for="message">Your Message:</label>
    <textarea class="form-control" id="message" name="message" placeholder="Enter your message" required></textarea>
  </div>
  
  <!-- Submit -->
  <button class="btn btn-primary" type="submit">Send</button>

  
</form>