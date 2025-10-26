# Jitsi Branding Removal Summary

## Changes Made

### 1. CSS Modifications
- Created `/css/no-branding.css` to hide all branding elements:
  - Watermarks (.watermark, .leftwatermark, .rightwatermark)
  - Powered by text (.poweredby)
  - Logo elements
  - Deep linking logos
  - Welcome page watermarks

### 2. Logo Image Replacements
Replaced the following logo images with transparent 1x1 pixel versions:
- `/images/watermark.svg` - transparent SVG
- `/images/jitsilogo.png` - transparent PNG
- `/images/logo-deep-linking.png` - transparent PNG
- `/images/logo-deep-linking-mobile.png` - transparent PNG

### 3. HTML Files Updated
Added reference to `css/no-branding.css` in the following files:

#### Main Files:
- `/index.html`

#### Static Pages:
- `/static/dialInInfo.html`
- `/static/prejoin.html`
- `/static/whiteboard.html`
- `/static/recommendedBrowsers.html`
- `/static/close2.html`
- `/static/close.html`
- `/static/404.html`

## Result
All Jitsi branding (logos, watermarks, powered-by text) has been removed from:
- Welcome/landing page
- Meeting room interface
- Pre-join screen
- Dial-in info pages
- All static pages

## How to Revert
If you need to restore branding:
1. Remove the `<link rel="stylesheet" href="css/no-branding.css">` line from all HTML files
2. Restore original logo images from backup
3. Delete `/css/no-branding.css`
