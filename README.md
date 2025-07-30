# Shopify Multicolumn Section

A flexible and responsive multicolumn section for Shopify themes that allows you to create beautiful column layouts with customizable content, images, and styling options.

## Features

- ✅ **Responsive Design**: Adapts seamlessly from desktop to mobile
- ✅ **Flexible Columns**: Support for 1-6 columns on desktop, 1-2 on mobile
- ✅ **Multiple Image Ratios**: Square, portrait, circle, and adaptive ratios
- ✅ **Mobile Slider**: Optional swipe functionality on mobile devices
- ✅ **Customizable Styling**: Multiple background styles and color schemes
- ✅ **Accessibility**: Full keyboard navigation and screen reader support
- ✅ **RTL Support**: Right-to-left language compatibility

## Installation

1. Copy `multicolumn.liquid` to your theme's `sections/` directory
2. Copy `section-multicolumn.css` to your theme's `assets/` directory
3. The section will automatically appear in your theme editor

## Files Included

```
sections/
└── multicolumn.liquid          # Main section file
assets/
└── section-multicolumn.css     # Styling for the section
```

## Usage

### Adding the Section

1. Go to your Shopify admin
2. Navigate to **Online Store > Themes**
3. Click **Customize** on your active theme
4. Add a section and select **Multicolumn**

### Customization Options

#### Section Settings

| Setting | Type | Options | Default | Description |
|---------|------|---------|---------|-------------|
| **Title** | Text | - | "Multicolumn" | Section heading |
| **Heading Size** | Select | Small, Medium, Large | Medium | Size of the section title |
| **Image Width** | Select | One third, Half, Full width | Full width | Width of column images |
| **Image Ratio** | Select | Adapt, Portrait, Square, Circle | Adapt | Aspect ratio for images |
| **Desktop Columns** | Range | 1-6 | 3 | Number of columns on desktop |
| **Column Alignment** | Select | Left, Center | Left | Text alignment in columns |
| **Background Style** | Select | None, Primary | Primary | Background styling |
| **Button Label** | Text | - | "Button label" | Call-to-action button text |
| **Button Link** | URL | - | - | Button destination URL |
| **Color Scheme** | Select | Theme colors | Background 1 | Section color scheme |

#### Mobile Settings

| Setting | Type | Options | Default | Description |
|---------|------|---------|---------|-------------|
| **Mobile Columns** | Select | 1, 2 | 1 | Columns on mobile devices |
| **Swipe on Mobile** | Checkbox | - | False | Enable slider on mobile |

#### Spacing Settings

| Setting | Type | Range | Default | Description |
|---------|------|-------|---------|-------------|
| **Top Padding** | Range | 0-100px | 36px | Space above section |
| **Bottom Padding** | Range | 0-100px | 36px | Space below section |

#### Column Block Settings

Each column can be customized with:

| Setting | Type | Description |
|---------|------|-------------|
| **Image** | Image Picker | Column image |
| **Title** | Rich Text | Column heading |
| **Text** | Rich Text | Column description |
| **Link Label** | Text | Button/link text |
| **Link** | URL | Button/link destination |

## Examples

### Basic 3-Column Layout

```liquid
<!-- This is automatically generated when you add the section -->
<div class="multicolumn">
  <!-- 3 columns with images, titles, and descriptions -->
</div>
```

### Features Showcase

Perfect for highlighting product features, services, or benefits:

1. **Column 1**: Image + "Fast Shipping" + Description + "Learn More" link
2. **Column 2**: Image + "Quality Products" + Description + "Shop Now" link  
3. **Column 3**: Image + "24/7 Support" + Description + "Contact Us" link

### Team Members

Great for about pages or team introductions:

1. **Column 1**: Team photo + Name + Role + Bio
2. **Column 2**: Team photo + Name + Role + Bio
3. **Column 3**: Team photo + Name + Role + Bio

## Responsive Behavior

### Desktop (750px+)
- Displays configured number of columns (1-6)
- Full grid layout with equal column widths
- Hover effects on cards

### Tablet (750px - 990px)
- Adapts column count for optimal viewing
- Maintains grid structure

### Mobile (<750px)
- Shows 1-2 columns as configured
- Optional slider functionality
- Touch-friendly navigation buttons

## Styling Customization

### CSS Variables

The section uses Shopify's CSS custom properties:

```css
/* Grid spacing */
--grid-desktop-horizontal-spacing
--grid-desktop-vertical-spacing
--grid-mobile-horizontal-spacing
--grid-mobile-vertical-spacing

/* Colors */
--color-background
--color-foreground
--color-border
--color-shadow

/* Typography */
--font-body-scale

/* Borders and shadows */
--text-boxes-radius
--text-boxes-border-width
--text-boxes-border-opacity
--text-boxes-shadow-opacity
```

### Custom Styling

To customize the appearance, you can override styles in your theme's CSS:

```css
/* Custom column card styling */
.multicolumn-card {
  border-radius: 1rem;
  transition: all 0.3s ease;
}

/* Custom hover effects */
.multicolumn-card:hover {
  transform: translateY(-0.5rem);
  box-shadow: 0 1rem 2rem rgba(0,0,0,0.1);
}

/* Custom image styling */
.multicolumn-card__image {
  filter: grayscale(100%);
  transition: filter 0.3s ease;
}

.multicolumn-card:hover .multicolumn-card__image {
  filter: grayscale(0%);
}
```

## Best Practices

### Content Guidelines

1. **Keep titles concise** - 2-4 words work best
2. **Limit text length** - 2-3 sentences per column
3. **Use consistent image sizes** - Same dimensions for all columns
4. **Optimize images** - Use WebP format when possible

### Design Tips

1. **Odd numbers** - 3 or 5 columns often look better than even numbers
2. **White space** - Don't fill every column; empty space improves readability
3. **Consistent styling** - Use the same image ratio across all columns
4. **Mobile-first** - Test on mobile devices regularly

### Performance

1. **Image optimization** - Compress images before uploading
2. **Lazy loading** - Shopify automatically handles this
3. **Minimal columns** - Avoid using 6 columns unless necessary

## Accessibility Features

- **Keyboard navigation** - Full tab support
- **Screen reader friendly** - Proper ARIA labels and semantic HTML
- **Focus indicators** - Clear visual focus states
- **Color contrast** - Follows WCAG guidelines
- **Alternative text** - Image alt attributes supported

## Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Troubleshooting

### Common Issues

**Images not displaying properly**
- Check image file format (JPG, PNG, WebP supported)
- Ensure images are uploaded to Shopify admin
- Verify image URLs are correct

**Layout breaking on mobile**
- Check mobile column settings
- Test with different device sizes
- Ensure CSS file is properly linked

**Slider not working**
- Enable "Swipe on Mobile" setting
- Check if JavaScript is enabled
- Verify slider component is loaded

### Support

For issues or questions:
1. Check the Shopify theme documentation
2. Test in different browsers
3. Verify all files are properly uploaded
4. Check browser console for errors

## License

This multicolumn section is provided as-is for use in Shopify themes. Feel free to modify and adapt it to your needs.

---

**Version**: 1.0.0  
**Compatible with**: Shopify Online Store 2.0 themes  
**Last updated**: 2024