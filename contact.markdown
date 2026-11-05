---
layout: default
title: "Tania Chapper M.A. - English Therapist in Mexico City"
permalink: /contact/
description: "Contact Tania Chapper, Experienced psychotherapist blending EMDR, Brainspotting, body movement for healing emotional, mental, and spiritual well-being. In English or Spanish."
---



<section>
  <div class="container">
  <h1 class="text-center mt-5 mb-4">Contact</h1>
    <div class="inside-container">
        <p class="page-intro">Trusting your mental, emotional, or spiritual wellbeing to someone new is no small thing. I get it because I’ve been on the other side of the therapy room myself. Degrees and certifications matter, but connection matters more. You can <a href="https://calendar.app.google/EfMBz7Kf5Y22KVur7" target="_blank" data-simple-event="book_session">book a session</a> so we can see if we genuinely click, with no pressure and no expectations.</p>
            <div class="blue-box form-container">
               <!-- 1. Include the EmailJS SDK -->
              <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>
              <!-- 2. Initialize EmailJS with your Public Key -->
              <script type="text/javascript">
                (function() {
                    // Replace with your actual EmailJS Public Key
                    emailjs.init("6wgfKuWQCwaLpsOI7");
                })();
              </script>
              <!-- 3. The Form (Notice there is no 'action' or 'method' attribute here) -->
              <form id="contact-form" class="custom-contact-form">
                <div class="form-group">
                  <label for="name">Name</label>
                  <!-- name attribute must match your EmailJS template variables (e.g., {{name}}) -->
                  <input type="text" id="name" name="name" required>
                </div>
                <div class="form-group">
                  <label for="email">Email</label>
                  <!-- name attribute must match your EmailJS template variables (e.g., {{email}}) -->
                  <input type="email" id="email" name="email" required>
                </div>
                <div class="form-group">
                  <label for="message">Message</label>
                  <!-- name attribute must match your EmailJS template variables (e.g., {{message}}) -->
                  <textarea id="message" name="message" rows="5" required></textarea>
                </div>
                <button type="submit" id="submit-button" class="box-button">Submit</button>
                <!-- A hidden status message that appears after submission -->
                <p id="form-status" style="display:none; text-align:center; margin-top:10px; font-size: 14px;"></p>
                <p class="privacy-disclaimer">
                  To protect your privacy, please refrain from sending sensitive personal information through this message thread.
                </p>
              </form>
              <!-- 4. The Script to handle the submission -->
              <script type="text/javascript">
                window.onload = function() {
                    document.getElementById('contact-form').addEventListener('submit', function(event) {
                        event.preventDefault(); // Prevents the default page refresh
                        const btn = document.getElementById('submit-button');
                        const statusText = document.getElementById('form-status');
                        btn.innerText = 'Sending...'; // Change button text while sending
                        // Replace with your EmailJS Service ID and Template ID
                        emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', this)
                            .then(function() {
                                btn.innerText = 'Submit';
                                statusText.style.display = 'block';
                                statusText.style.color = 'green';
                                statusText.innerText = 'Message sent successfully!';
                                document.getElementById('contact-form').reset(); // Clear the form
                            }, function(error) {
                                btn.innerText = 'Submit';
                                statusText.style.display = 'block';
                                statusText.style.color = 'red';
                                statusText.innerText = 'Failed to send message. Please try again.';
                                console.log('EmailJS Error:', error);
                            });
                    });
                }
              </script>
            </div>
    </div>
  </div>
</section>