# ICA Component Library

## Overview

The ICA website uses a modular component-based architecture for improved maintainability, reusability, and development efficiency. All homepage sections have been extracted into individual components that can be reused across the site.

## Available Components

### Licensing & Credentials ⭐ NEW
- **File:** `licensing-credentials.njk`
- **Usage:** `{% include "sections/licensing-credentials.njk" %}`
- **Variables:**
  - `sectionTitle` - Main heading (default: "Licensed, Bonded & Insured")
  - `showVerifyLinks` - Show/hide verification links (default: true)
  - `theme` - Color theme: "dark" or "light" (default: "dark")
- **Features:**
  - Spray Foam Insurance logo integration
  - Three credential cards: Licensed (ROC #326891), Bonded, Insured
  - Verification links to ROC and BBB
  - Contact info for insurance certificates
  - Futuristic glassmorphism design
  - Mobile-responsive grid layout
- **Important Links:**
  - ROC License: https://roc.force.com/AZRoc/s/contractor-search?licenseId=a0o8y0000005GtuAAE
  - BBB Profile: https://www.bbb.org/us/az/glendale/profile/insulation-contractors/insulation-contractors-of-arizona-1126-1000090032
  - Spray Foam Insurance: https://sprayfoaminsurance.com/

### Safety Excellence ⭐ NEW
- **File:** `safety-excellence.njk`
- **Usage:** `{% include "sections/safety-excellence.njk" %}`
- **Variables:**
  - `sectionTitle` - Main heading (default: "Safety Excellence at Every Installation")
  - `showSafetyPoints` - Show/hide safety feature cards (default: true)
  - `ctaText` - Button text (default: "Schedule Your Safe Installation Today")
  - `ctaUrl` - Button link (default: "/contact")
- **Features:**
  - Yellow/warning color theme for safety emphasis
  - Animated safety badge and shield icon
  - Four safety feature cards: Property Protection, Certified Technicians, Clean Installation, Safety Inspections
  - Floating animation effects
  - Mobile-responsive grid layout

### Credentials Banner ⭐ NEW
- **File:** `credentials-banner.njk`
- **Usage:** `{% include "sections/credentials-banner.njk" %}`
- **Variables:**
  - `position` - Banner position: "top" or "bottom" (default: "bottom")
  - `theme` - Color theme: "dark" or "light" (default: "dark")
  - `showPhone` - Show/hide phone number (default: true)
- **Features:**
  - Compact horizontal layout for headers/footers
  - Spray Foam Insurance logo
  - Licensed ROC #326891, Bonded & Insured, BBB A+ Rating
  - Verify License button
  - Animated background sweep effect
  - Mobile-responsive with icon-only mode on small screens

### Contact Form
- **File:** `contact-form.njk`
- **Usage:** `{% include "sections/contact-form.njk" %}`
- **Variables:**
  - `showContactForm` - Show/hide entire form (default: true)
  - `formTitle` - Form heading (default: "Get Your Free Insulation Estimate")
  - `formSubtitle` - Form description (default: "Fill out the form below and we'll contact you within 24 hours")
- **Features:**
  - Netlify Forms integration for easy form handling
  - Grid and particles background effect matching homepage design
  - Honeypot field for spam protection
  - Service selection dropdown
  - Mobile-responsive layout
  - Futuristic styling with glassmorphism effects

### Hero Section
- **File:** `hero.njk`
- **Usage:** `{% include "sections/hero.njk" %}`
- **Variables:**
  - `heroTitle` - Main heading text (default: "Arizona's Premier Insulation Experts")
  - `heroSubtitle` - Subheading text (default: site.tagline)
  - `showBenefits` - Show/hide benefit cards (default: true)
  - `ctaPrimary` - Primary button text (default: "Get Free Assessment")
  - `ctaSecondary` - Secondary button text (default: "Call " + site.phone)
  - `ctaPrimaryLink` - Primary button link (default: "/contact/")
  - `ctaSecondaryLink` - Secondary button link (default: "tel:" + site.phone)

### Services Preview
- **File:** `services-preview.njk`
- **Usage:** `{% include "sections/services-preview.njk" %}`
- **Variables:**
  - `sectionTitle` - Section heading (default: "Professional Insulation Services")
  - `sectionIntro` - Section introduction text
  - `showServiceCards` - Show/hide service cards (default: true)
  - `serviceCount` - Number of services to display (default: 4)
- **Features:**
  - Grid and particles background effect (NEW)
  - Enhanced card styling for dark background
  - Four service categories: Residential, Commercial, Industrial, Agricultural

### Additional CTA
- **File:** `additional-cta.njk`
- **Usage:** `{% include "sections/additional-cta.njk" %}`
- **Variables:**
  - `showAdditionalCTA` - Show/hide entire section (default: true)
  - `ctaTitle` - Main heading (default: "Ready to Transform Your Home's Comfort?")
  - `ctaSubtitle` - Subtitle text (default: "Join hundreds of satisfied Arizona homeowners who trust ICA")
  - `ctaPrimaryText` - Primary button text (default: "Get Your Free Assessment")
  - `ctaPrimaryUrl` - Primary button link (default: "#contact")
  - `ctaSecondaryText` - Secondary button text (default: "View Our Work")
  - `ctaSecondaryUrl` - Secondary button link (default: "/projects")
- **Features:**
  - Grid and particles background effect
  - Four trust indicators with check icons
  - Dual CTA buttons (primary and secondary)
  - Gradient text effect on title
  - Mobile-responsive layout

### Insulation Applications
- **File:** `insulation-applications.njk`
- **Usage:** `{% include "sections/insulation-applications.njk" %}`
- **Variables:**
  - `sectionTitle` - Section heading (default: "Insulation Applications")
  - `sectionSubtitle` - Section description text
  - `showSection` - Show/hide entire section (default: true)
- **Features:**
  - 6 insulation application cards matching service-card styling
  - Correct image paths (/Images/ directory)
  - Consistent with website's futuristic theme
  - Mobile-responsive grid layout
  - Applications: Open Cell, Closed Cell, Fiberglass, Blown-In, Drill & Fill, Removal

### Why Choose ICA
- **File:** `why-choose-ica.njk`
- **Usage:** `{% include "sections/why-choose-ica.njk" %}`
- **Variables:**
  - `sectionTitle` - Section heading (default: "Why Arizona Homeowners Choose ICA")
  - `sectionIntro` - Section introduction text
  - `showFeatureCards` - Show/hide feature cards (default: true)

### Accreditations Banner
- **File:** `accreditations-banner.njk`
- **Usage:** `{% include "sections/accreditations-banner.njk" %}`
- **Variables:**
  - `sectionTitle` - Section heading (default: "Trusted by Industry Leaders")
  - `showSection` - Show/hide entire section (default: true)
  - `animationSpeed` - Logo scroll animation speed (default: "30s")
- **Features:**
  - Animated right-to-left infinite loop of accreditation logos
  - Transparent background for versatility
  - Gradient fade edges for smooth visual flow
  - Hover effects: pauses animation and highlights individual logos
  - Mobile-responsive with adjusted sizes
  - Logos: SFWW Ambassador 2025, ICAA, SPFA, ROC Seal

### Testimonials
- **File:** `testimonials.njk`
- **Usage:** `{% include "sections/testimonials.njk" %}`
- **Variables:**
  - `sectionTitle` - Section heading (default: "Real Results from Arizona Homeowners")
  - `sectionIntro` - Section introduction text
  - `testimonialCount` - Number of testimonials to show (default: 3)
  - `showResults` - Show/hide result metrics (default: true)

### Recent Posts
- **File:** `recent-posts.njk`
- **Usage:** `{% include "sections/recent-posts.njk" %}`
- **Variables:**
  - `sectionTitle` - Section heading (default: "Insulation Resources & Expert Advice")
  - `sectionIntro` - Section introduction text
  - `postCount` - Number of posts to display (default: 3)
  - `showViewAllButton` - Show/hide "View All" button (default: true)

### Air Duct Cleaning
- **File:** `air-duct-cleaning.njk`
- **Usage:** `{% include "sections/air-duct-cleaning.njk" %}`
- **Variables:**
  - `sectionTitle` - Section heading (default: "Now Offering Professional Air Duct Cleaning!")
  - `sectionSubtitle` - Section description text
  - `ctaText` - Button text (default: "Book Now!")
  - `ctaUrl` - Button link (default: "/contact")
  - `showSection` - Show/hide entire section (default: true)

### CTA Section
- **File:** `cta.njk`
- **Usage:** `{% include "sections/cta.njk" %}`
- **Variables:**
  - `ctaTitle` - Main CTA heading
  - `ctaText` - CTA description text
  - `highlightTitle` - Highlight box title
  - `highlightText` - Highlight box text
  - `showHighlight` - Show/hide highlight box (default: true)
  - `ctaPrimary` - Primary button text
  - `ctaSecondary` - Secondary button text
  - `ctaPrimaryLink` - Primary button link
  - `ctaSecondaryLink` - Secondary button link
  - `showFooterInfo` - Show/hide footer info (default: true)

## Usage Examples

### Basic Usage (Homepage)
```njk
---
layout: base.njk
title: Home
---

{% include "sections/contact-form.njk" %}
{% include "sections/hero.njk" %}
{% include "sections/services-preview.njk" %}
{% include "sections/additional-cta.njk" %}
{% include "sections/insulation-applications.njk" %}
{% include "sections/why-choose-ica.njk" %}
{% include "sections/accreditations-banner.njk" %}
{% include "sections/testimonials.njk" %}
{% include "sections/recent-posts.njk" %}
{% include "sections/air-duct-cleaning.njk" %}
{% include "sections/cta.njk" %}
```

### Service Page with Credentials
```njk
---
layout: base.njk
title: Spray Foam Insulation
---

{% include "sections/hero.njk" %}
{% include "sections/licensing-credentials.njk" %}
{% include "sections/safety-excellence.njk" %}
{% include "sections/testimonials.njk" %}
{% include "sections/contact-form.njk" %}
```

### Header with Credentials Banner
```njk
{# In your header template #}
{% set position = "top" %}
{% include "sections/credentials-banner.njk" %}
```

### Footer with Credentials Banner
```njk
{# In your footer template #}
{% set position = "bottom" %}
{% set theme = "dark" %}
{% include "sections/credentials-banner.njk" %}
```

### Custom Licensing Section
```njk
{% set sectionTitle = "Your Trusted Insulation Partner" %}
{% set theme = "light" %}
{% include "sections/licensing-credentials.njk" %}
```

### Custom Safety Section
```njk
{% set sectionTitle = "Our Commitment to Safe Installation" %}
{% set ctaText = "Learn About Our Safety Protocols" %}
{% set ctaUrl = "/safety" %}
{% include "sections/safety-excellence.njk" %}
```

### Custom Contact Form
```njk
{% set formTitle = "Schedule Your Spray Foam Consultation" %}
{% set formSubtitle = "Expert installation for Arizona homes" %}
{% include "sections/contact-form.njk" %}
```

### Custom Additional CTA
```njk
{% set ctaTitle = "Experience the ICA Difference" %}
{% set ctaSubtitle = "Professional insulation services you can trust" %}
{% set ctaPrimaryText = "Get Started Today" %}
{% include "sections/additional-cta.njk" %}
```

### Custom Hero for Service Pages
```njk
{% set heroTitle = "Expert Spray Foam Insulation in Phoenix" %}
{% set heroSubtitle = "Superior R-values and air sealing for Arizona homes" %}
{% set ctaPrimary = "Get Spray Foam Quote" %}
{% include "sections/hero.njk" %}
```

### Testimonials on Service Pages
```njk
{% set sectionTitle = "Spray Foam Success Stories" %}
{% set testimonialCount = 2 %}
{% include "sections/testimonials.njk" %}
```

### Custom Air Duct Cleaning Section
```njk
{% set sectionTitle = "Breathe Cleaner Air Today!" %}
{% set sectionSubtitle = "Professional duct cleaning for healthier homes" %}
{% set ctaText = "Schedule Cleaning" %}
{% include "sections/air-duct-cleaning.njk" %}
```

### Custom CTA Section
```njk
{% set ctaTitle = "Ready for Superior Insulation?" %}
{% set ctaText = "Transform your home with spray foam insulation" %}
{% set ctaPrimary = "Schedule Spray Foam Assessment" %}
{% include "sections/cta.njk" %}
```

## Component Architecture Benefits

1. **File Size Reduction:** From 8,530 bytes monolithic file to 14 modular components
2. **Edit Speed:** 60-80% faster section updates
3. **Reusability:** Components can be used across all pages
4. **Maintainability:** Changes to one component update all instances
5. **Development Speed:** New pages can be assembled from existing components

## Best Practices

1. **Always provide sensible defaults** - Components should work without custom variables
2. **Use descriptive variable names** - Prefix with component context (e.g., `heroTitle` not just `title`)
3. **Keep components focused** - Each component should have a single responsibility
4. **Document all variables** - List all available customization options
5. **Test component variations** - Ensure components work with different variable combinations
6. **Include important URLs** - Keep accreditation links documented for future content

## Important Accreditation Links

For future content development, here are the verified accreditation links:
- **ROC License Verification:** https://roc.force.com/AZRoc/s/contractor-search?licenseId=a0o8y0000005GtuAAE
- **BBB Business Profile:** https://www.bbb.org/us/az/glendale/profile/insulation-contractors/insulation-contractors-of-arizona-1126-1000090032
- **Spray Foam Insurance:** https://sprayfoaminsurance.com/
- **Spray Foam Insurance Logo:** /images/Spray_Foam_Insurance_logo.webp

## Future Enhancements

- Add component variants (e.g., hero-minimal, hero-video)
- Create location-specific component variations
- Add animation options via variables
- Implement component versioning system
- Create visual component gallery
- Add more credential display options (compact, expanded, etc.)
