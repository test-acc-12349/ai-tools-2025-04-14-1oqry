# AI Tools Directory 🤖

> The ultimate directory of AI tools and resources for professionals and enthusiasts.

[![Netlify Status](https://api.netlify.com/api/v1/badges/xxxxx-xxxxx-xxxxx/deploy-status)](https://app.netlify.com/sites/aitools/deploys)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview

AI Tools is a comprehensive directory website showcasing the latest artificial intelligence tools and resources in a clean, responsive 3-column grid layout. The directory is designed to be easily customizable and maintainable.

## Features

- 🎯 Responsive 3-column grid layout
- 🔍 Search functionality
- 🏷️ Category filtering
- 💨 Fast loading times
- 📱 Mobile-friendly design
- 🎨 Customizable styling
- 🔗 SEO-friendly URLs

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── src/
│   ├── components/
│   │   ├── Card.js
│   │   ├── Grid.js
│   │   └── Hero.js
│   ├── data/
│   │   └── tools.json
│   ├── styles/
│   │   └── main.css
│   └── pages/
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization Guide

### Adding Directory Items

Edit `src/data/tools.json`:

```json
{
  "tools": [
    {
      "id": "tool-1",
      "name": "AI Tool Name",
      "description": "Tool description",
      "category": "Category",
      "url": "https://example.com",
      "image": "/images/tool-image.png"
    }
  ]
}
```

### Modifying Categories

Update categories in `src/data/categories.js`:

```javascript
export const categories = [
  "Machine Learning",
  "Natural Language Processing",
  "Computer Vision",
  "Robotics"
];
```

### Customizing Hero Section

Edit `src/components/Hero.js`:

```javascript
const Hero = () => {
  return (
    <div className="hero">
      <h1>Your Custom Title</h1>
      <p>Your custom description</p>
    </div>
  );
};
```

### Styling Customization

Modify `src/styles/main.css`:

```css
:root {
  --primary-color: #007bff;
  --secondary-color: #6c757d;
  --background-color: #ffffff;
}
```

## Deployment

### Netlify Deployment

1. Push your repository to GitHub
2. Login to Netlify
3. Click "New site from Git"
4. Select your repository
5. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
6. Click "Deploy site"

## Custom Domain Setup

1. Purchase domain from your preferred registrar
2. In Netlify:
   - Go to Site settings > Domain management
   - Click "Add custom domain"
   - Enter your domain name
3. Configure DNS settings:
   - Add CNAME record pointing to your Netlify URL
   - Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. **Build Failures**
   - Verify Node.js version
   - Check for dependency conflicts
   - Review build logs

2. **Styling Issues**
   - Clear browser cache
   - Check CSS specificity
   - Verify media queries

3. **Search Not Working**
   - Check JavaScript console
   - Verify data structure
   - Review search implementation

## Support & Resources

- [Documentation](https://docs.example.com)
- [GitHub Issues](https://github.com/yourusername/ai-tools-directory/issues)
- [Community Forum](https://forum.example.com)
- [Email Support](mailto:support@example.com)

### Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

Made with ❤️ by [Your Name](https://github.com/yourusername)