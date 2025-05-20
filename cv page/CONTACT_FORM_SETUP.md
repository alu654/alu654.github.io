# Contact Form Setup Instructions

The contact form on your CV page is now configured to send data to a form handling service. Follow these instructions to make it fully functional:

## Option 1: Using Formspree (Recommended for Beginners)

1. Go to [Formspree](https://formspree.io/) and create a free account
2. Create a new form in your Formspree dashboard
3. Copy the unique form ID provided by Formspree
4. Open the `js/main.js` file and locate the `initContactForm()` function
5. Replace `your-formspree-id` in the fetch URL with your actual Formspree form ID:

```javascript
fetch('https://formspree.io/f/your-formspree-id', {
```

That's it! Your form will now send messages to your email through Formspree.

## Option 2: Using Your Own Backend

If you prefer to handle form submissions with your own server:

1. Create a server endpoint that accepts POST requests with JSON data
2. Update the fetch URL in `js/main.js` to point to your server endpoint:

```javascript
fetch('https://your-server.com/api/contact', {
```

3. Ensure your server properly handles the following JSON fields:
   - `name`
   - `email`
   - `subject`
   - `message`

## Testing the Form

After setting up either option:

1. Open your CV page in a browser
2. Fill out the contact form
3. Submit the form
4. You should see the "Sending..." text while the form is being submitted
5. Upon successful submission, you'll see a success message

## Troubleshooting

If the form isn't working:

1. Check the browser console for any JavaScript errors
2. Verify that your Formspree ID or server URL is correct
3. Ensure your server is properly configured to handle CORS if using your own backend

For additional help, refer to [Formspree's documentation](https://formspree.io/docs/) or consult your server's API documentation.