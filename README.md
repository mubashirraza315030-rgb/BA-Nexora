# BA Nexora AI 🚀

BA Nexora AI is a premium, futuristic landing page and digital showcase built for an AI startup. It features a highly aesthetic "glassmorphic" design, dynamic JavaScript-driven modals, an integrated WhatsApp CRM, and a local admin dashboard.

## 🌟 Features

- **Modern UI/UX**: Uses Tailwind CSS to achieve a state-of-the-art dark mode aesthetic with glowing neon gradients, glass panels, and ambient animations.
- **Dynamic Service Modals**: Clickable service cards that open fully responsive modals detailing service benefits, examples, and technologies.
- **WhatsApp Integration**: A floating WhatsApp button and a Contact Form that automatically formats user inquiries and forwards them directly to the business's WhatsApp.
- **Admin Dashboard (`admin.html`)**: A secure, local-storage-powered dashboard that automatically intercepts and saves form submissions so leads are never lost.
- **Project Showcase (`projects.html`)**: A dedicated portfolio page with a JavaScript array system allowing developers to easily inject new project cards and multi-media galleries.

---

## 🛠️ Tech Stack

- **HTML5** & **Vanilla JavaScript** (No heavy frameworks required)
- **Tailwind CSS** (via CDN for rapid styling and responsive design)
- **Google Fonts** (Space Grotesk, Inter, JetBrains Mono)
- **Google Material Symbols** (Icons)

---

## 🧑‍💻 Developer Guide

This project is designed to be easily configurable without complex build steps.

### 1. Setting the WhatsApp Number
To receive messages from the contact form directly to your phone, you must update the WhatsApp number in `code.html`.
- Open `code.html`.
- Scroll to the `<script>` tag at the bottom.
- Find the constant `WHATSAPP_NUMBER` and replace `"1234567890"` with your actual business phone number (include the country code, no + or spaces).
```javascript
const WHATSAPP_NUMBER = "1yourphonenumber"; // SET WHATSAPP NUMBER HERE
```

### 2. Adding New Projects to the Showcase
The `projects.html` page is driven by a simple JavaScript array. You do not need to copy and paste complex HTML to add new projects.
- Open `projects.html`.
- Locate the `projectsData` array inside the `<script>` block.
- Add a new object to the array with your project details. You can add as many images or videos as you want to the `media` array.
```javascript
{
    id: "unique-project-id",
    name: "My Awesome Project",
    category: "AI Software",
    description: "A brief description of what this project does.",
    media: [
        { type: "image", url: "https://link-to-your-image.png" },
        { type: "video", url: "https://link-to-your-video.mp4" }
    ]
}
```

### 3. Managing Contact Form Submissions (Admin)
The contact form uses the browser's `localStorage` to save submissions locally under the key `nexora_messages`.
- To view saved messages, navigate to `admin.html` in your browser.
- You can individually delete messages or clear the entire inbox from this UI.
- *Note: Since this uses `localStorage`, data is unique to the browser it was submitted on. For production deployment across multiple users, replace the `localStorage` logic in `handleContactSubmit` with a real backend API call.*

---

## 🚀 Running Locally

Because this project uses vanilla web technologies and a CDN for Tailwind CSS, you do not need to install `npm` modules.
Simply double-click `code.html` to open it in any modern web browser. 

For the best experience when testing `localStorage` and routing, it is recommended to serve the directory using a local web server:
```bash
# If using Python:
python -m http.server 8000

# If using Node.js:
npx serve .
```

Enjoy building the future! 🧠✨
