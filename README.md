# Servland - Business Landing Page Theme

A modern, responsive business landing page theme built with Astro and Tailwind CSS. Perfect for businesses looking for an effective and speedy online presence.

![Servland Preview](preview.png)

## 🚀 Features

- ⚡️ **Lightning Fast**: Built with Astro for optimal performance
- 🎨 **Beautiful Design**: Modern UI with Tailwind CSS
- 🌗 **Dark Mode**: Automatic and manual dark mode support
- 📱 **Fully Responsive**: Looks great on all devices
- 📧 **Contact Form**: Integrated with EmailJS or Nodemailer
- 💬 **WhatsApp Integration**: Direct messaging capability
- 🍪 **Cookie Consent**: GDPR-compliant cookie banner
- 🖼️ **Parallax Effects**: Engaging background animations
- 🔍 **SEO Ready**: Optimized meta tags and structured data
- 🛠️ **Easy to Customize**: Well-organized code structure

## 🛠️ Quick Start

1. **Clone the repository**
```bash
git clone https://github.com/locobean/servland.git
cd servland
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
```bash
cp .env.example .env
```

4. **Start development server**
```bash
npm run dev
```

Visit `http://localhost:4321` to see your site!

## 📧 Email Configuration

### Option 1: EmailJS (Recommended for Static Sites)

1. Create an account at [EmailJS](https://www.emailjs.com/)
2. Create an email template with variables:
   - `{{name}}` - Sender's name
   - `{{email}}` - Sender's email
   - `{{tel}}` - Phone number
   - `{{message}}` - Message content
3. Add credentials to `.env`:
```env
PUBLIC_EMAILJS_SERVICE_ID=your-service-id
PUBLIC_EMAILJS_TEMPLATE_ID=your-template-id
PUBLIC_EMAILJS_USER_ID=your-public-key
```

### Option 2: Nodemailer with SMTP

1. Configure SMTP settings in `.env`:
```env
EMAIL_USERNAME=your-email@example.com
EMAIL_PASSWORD=your-app-specific-password
RECIPIENT_EMAIL=recipient@example.com
SECRET_KEY=your-secret-key-for-hashing
```

For Gmail, use an [App-Specific Password](https://support.google.com/accounts/answer/185833).

## 🎨 Customization

### Content
- Edit main content in `src/pages/index.astro`
- Modify components in `src/components/`
- Update styles in `tailwind.config.mjs`

### Styling
- Colors: Update `tailwind.config.mjs`
- Typography: Modify font imports in `Layout.astro`
- Components: Edit individual component files

### Images
- Replace `public/preview.png` with your site preview
- Update favicon in `public/favicon.svg`

## 📦 Building for Production

1. **Build the site**
```bash
npm run build
```

2. **Preview the build**
```bash
npm run preview
```

The built files will be in the `dist/` directory.

## ☁️ Cloudflare Pages Deployment

This site is optimized for Cloudflare Pages deployment. See [CLOUDFLARE_DEPLOYMENT.md](CLOUDFLARE_DEPLOYMENT.md) for detailed instructions.

**Quick Deploy:**
1. Connect your repository to Cloudflare Pages
2. Use build command: `npm run build`
3. Set build output directory: `dist`
4. Deploy!

## 🚀 Recent Improvements

### Performance Optimizations
- ✅ Cloudflare Pages adapter configured for hybrid rendering
- ✅ Optimized font loading (non-blocking)
- ✅ Lazy loading for calendar iframe
- ✅ Improved parallax background with `requestAnimationFrame`
- ✅ Added `prefers-reduced-motion` support
- ✅ CSS minification with Lightning CSS

### WhatsApp Integration
- ✅ Fixed WhatsApp link with pre-filled message
- ✅ Added floating WhatsApp button for mobile
- ✅ Proper URL encoding for Spanish characters

### Background Improvements
- ✅ Increased opacity from 0.15 to 0.35 for better visibility
- ✅ Removed excessive blur effect
- ✅ Added professional gradient overlays
- ✅ Optimized animations for performance

### Mobile Enhancements
- ✅ Responsive calendar iframe
- ✅ Floating WhatsApp button with pulse animation
- ✅ Touch-optimized UI elements
- ✅ Improved mobile performance

See [IMAGE_OPTIMIZATION_GUIDE.md](IMAGE_OPTIMIZATION_GUIDE.md) for image optimization recommendations.

## 🤝 Contributing

Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md).

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 💖 Support

- Star this repository
- Report issues
- Follow for updates

---

Made with ❤️ by [locobean](https://github.com/locobean)
