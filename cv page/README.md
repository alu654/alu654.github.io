# Interactive CV Website

This is a modern, interactive CV/Resume website built with HTML, CSS, and JavaScript. It features a responsive design, smooth animations, and interactive elements to showcase your professional experience in an engaging way.

## Features

- Responsive design that works on all devices
- Smooth scrolling navigation
- Animated sections that reveal as you scroll
- Interactive skill bars
- Project filtering by category
- Contact form
- Modern and clean UI

## Getting Started

### Prerequisites

No special prerequisites are needed. You can edit this website with any text editor and view it in any modern web browser.

### Customization

1. **Personal Information**:
   - Open `index.html` and replace the placeholder text with your information
   - Update your name, title, and professional summary in the hero section
   - Add your contact information in the contact section

2. **Profile Picture**:
   - Replace the placeholder image at `img/profile.jpg` with your own photo
   - For best results, use a square image (recommended size: 500x500px)

3. **Background Image**:
   - Replace the hero background at `img/hero-bg.jpg` with your preferred image

4. **Experience & Education**:
   - Update the timeline items in the Experience section with your work history
   - Update the education items with your educational background

5. **Skills**:
   - Modify the skill bars in the Skills section to reflect your expertise levels
   - Update the skill tags to showcase your soft skills

6. **Projects**:
   - Add your own projects with descriptions and links
   - Update the project categories in both the HTML and JavaScript filter buttons
   - Replace project images in the `img/` folder

7. **Colors & Styling**:
   - To change the color scheme, edit the CSS variables in the `:root` section of `css/styles.css`

## File Structure

```
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # All styles
├── js/
│   └── main.js         # JavaScript functionality
└── img/                # Image directory
    ├── profile.jpg     # Your profile picture
    ├── hero-bg.jpg     # Hero section background
    ├── project1.jpg    # Project images
    └── project2.jpg
```

## Usage

To view the website locally, simply open the `index.html` file in your web browser.

To deploy the website, upload all files to your web hosting service.

## Customizing the Contact Form

The contact form currently displays an alert message when submitted. To make it functional:

1. Create a server-side script to handle form submissions (PHP, Node.js, etc.)
2. Update the `initContactForm()` function in `main.js` to send data to your server

## License

Feel free to use this template for your personal CV/Resume website.

## Acknowledgments

* Font Awesome for the icons
* Google Fonts for typography