# Shopify Swipeable Image Gallery Section

A fully responsive, swipeable image gallery section for Shopify themes with touch/mouse support and customizable settings.

## ✨ Features

- **Responsive Design**: 4 columns on desktop, adaptive on mobile (fully customizable)
- **Swipe Functionality**: Touch gestures on mobile, click & drag on desktop
- **Smart Navigation**: 
  - Arrows on desktop only (can be disabled)
  - Dots on both desktop and mobile (can be disabled)
  - Auto-hide when not needed
- **Shopify Integration**: Full theme customizer support with live preview
- **Performance Optimized**: Lazy loading, smooth animations, minimal JavaScript
- **Customizable**: Colors, spacing, aspect ratios, column counts, and more

## 📋 Specifications

- **Max Width**: 1800px (customizable: 1200px - 2000px)
- **Desktop Padding**: 55px horizontal (customizable: 20px - 100px)
- **Default Columns**: 4 desktop, 3 tablet, 2 mobile, 1 small mobile
- **Image Aspect Ratios**: Square, Landscape, Portrait, Wide
- **Navigation**: Arrows (desktop) + Dots (both) with smart hiding

## 🚀 Installation

### Method 1: Direct Upload
1. Download `swipeable-gallery.liquid`
2. In your Shopify admin, go to **Online Store > Themes**
3. Click **Actions > Edit code** on your active theme
4. Navigate to **Sections** folder
5. Click **Add a new section**
6. Name it `swipeable-gallery` and paste the code
7. Save the file

### Method 2: Theme Development
1. Clone your theme repository
2. Add `swipeable-gallery.liquid` to the `/sections/` directory
3. Deploy to your theme

## 📖 Usage

### Adding to Pages
1. Go to **Online Store > Themes > Customize**
2. Navigate to the page where you want to add the gallery
3. Click **Add section**
4. Select **Swipeable Image Gallery**
5. Configure settings and add images

### Adding Images
1. In the section settings, click **Add Gallery Image**
2. Upload or select images from your media library
3. Repeat for all desired images
4. Images will automatically organize into swipeable pages

### Customization Options

#### Layout Settings
- **Maximum Width**: 1200px - 2000px (default: 1800px)
- **Desktop Padding**: 20px - 100px (default: 55px)
- **Mobile Padding**: 10px - 50px (default: 20px)

#### Column Configuration
- **Desktop**: 2-6 columns (default: 4)
- **Tablet**: 2-4 columns (default: 3)
- **Mobile**: 1-3 columns (default: 2)
- **Small Mobile**: 1-2 columns (default: 1)

#### Navigation Options
- **Show Arrows**: Toggle desktop navigation arrows
- **Show Dots**: Toggle dot navigation for all devices

#### Styling Options
- **Image Aspect Ratio**: Square, Landscape, Portrait, Wide
- **Background Colors**: Section and gallery backgrounds
- **Border Radius**: 0-30px rounded corners
- **Gap Size**: 10-40px spacing between images
- **Section Spacing**: Top and bottom padding

## 🎨 Customization Examples

### Gallery Styles
```liquid
<!-- Square images with tight spacing -->
aspect_ratio: "1/1"
gap_size: 10
border_radius: 8

<!-- Wide landscape gallery -->
aspect_ratio: "16/9"
desktop_columns: 3
gap_size: 30
```

### Responsive Behavior
```liquid
<!-- Mobile-first design -->
desktop_columns: 3
tablet_columns: 2
mobile_columns: 1
small_mobile_columns: 1

<!-- Dense desktop layout -->
desktop_columns: 6
tablet_columns: 4
mobile_columns: 3
small_mobile_columns: 2
```

## 🔧 Technical Details

### Browser Support
- **Modern Browsers**: Chrome, Firefox, Safari, Edge (latest 2 versions)
- **Mobile**: iOS Safari, Chrome Mobile, Samsung Internet
- **Touch Support**: Full touch gesture support on all devices

### Performance Features
- **Lazy Loading**: Images load as needed
- **Smooth Animations**: Hardware-accelerated CSS transitions
- **Efficient Rendering**: Minimal DOM manipulation
- **Responsive Images**: Shopify's responsive image system

### Accessibility
- **Keyboard Navigation**: Arrow keys and tab support
- **Screen Readers**: Proper ARIA labels and alt text
- **Focus Management**: Visible focus indicators
- **Reduced Motion**: Respects user motion preferences

## 🐛 Troubleshooting

### Common Issues

**Gallery not showing:**
- Ensure images are uploaded in the section blocks
- Check that the section is added to the page template

**Swipe not working:**
- Verify JavaScript is enabled
- Check for console errors
- Ensure the section has a unique ID

**Images not loading:**
- Confirm images are properly uploaded to Shopify
- Check image file formats (JPG, PNG, WebP supported)
- Verify image URLs are accessible

**Responsive issues:**
- Clear browser cache
- Test on actual devices, not just browser resize
- Check theme CSS conflicts

### Performance Optimization
- Use appropriately sized images (recommended: 800px width)
- Enable Shopify's image optimization
- Limit the number of images per gallery (recommended: 20-30 max)

## 📱 Mobile Behavior

- **Touch Gestures**: Swipe left/right to navigate
- **No Arrows**: Navigation arrows hidden on mobile
- **Dots Only**: Dot navigation for page indication
- **Responsive Columns**: Automatically adjusts column count
- **Touch Feedback**: Visual feedback on touch interactions

## 🎯 Best Practices

### Image Guidelines
- **Dimensions**: Use consistent aspect ratios
- **File Size**: Optimize images (under 500KB recommended)
- **Alt Text**: Add descriptive alt text for accessibility
- **Quality**: Use high-quality images for best results

### Content Strategy
- **Image Count**: 8-20 images work best for user engagement
- **Consistency**: Use similar lighting and style
- **Order**: Arrange images in logical sequence
- **Updates**: Regularly refresh gallery content

### Performance Tips
- **Lazy Loading**: Enabled by default, don't disable
- **Image Optimization**: Use Shopify's image transformation
- **Caching**: Leverage browser caching for repeat visitors
- **Testing**: Test on various devices and connection speeds

## 🔄 Updates & Maintenance

### Version History
- **v1.0**: Initial release with full functionality
- **Future**: Planned features include video support, lightbox integration

### Maintenance
- **Regular Testing**: Test functionality after theme updates
- **Image Cleanup**: Remove unused images to improve performance
- **Settings Review**: Periodically review and optimize settings

## 📞 Support

For issues or questions:
1. Check the troubleshooting section above
2. Test in a development theme first
3. Verify Shopify theme compatibility
4. Check browser console for JavaScript errors

## 📄 License

This section is provided as-is for Shopify theme development. Feel free to modify and customize for your specific needs.

---

**Ready to enhance your Shopify store with a beautiful, swipeable image gallery!** 🎉