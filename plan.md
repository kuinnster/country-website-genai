# Country Website Implementation Plan

## Objective

Build a polished, responsive, accessible, multi-page website for one location from a blank workspace. The project will use plain HTML and CSS only (apart from a normalizing/reset stylesheet), include licensed multimedia and content, and provide complete source-attribution documentation.

## Project Preferences

- Location: Colombia
- Three location-page topics:
  - Major attractions (serving as `index.html`, the main entry point)
  - Culture and traditions
  - Food and cuisine
- Visual direction: bold and colorful
- AI use: planning, copy, and code assistance, with final user review
- Existing brand assets or constraints: none
- Contact form: static accessible demo only; no data submission or backend functionality
- GitHub publication: handled by the user

## Approach

1. **Choose and scope the location**
   - Select a country, city, continent, or fictional location before implementation.
   - Define a concise content theme and identify the subjects for the three location pages.
   - Use a coherent page structure and original copy that can be supported by Creative Commons licensed sources.

2. **Plan the visual and content structure**
   - Create mobile-first wireframes for the three location pages (`index.html`, culture, and food) and the credits page.
   - Map required HTML elements to specific pages during wireframing so each page has clear content balance:
     - **Major Attractions (`index.html`):** Hero/featured image and the accessible contact/inquiry form.
     - **Culture & Traditions:** Blockquote and an audio player featuring the bambuco excerpt “Cuando la vida se va,” credited to Alexander Cuesta-Moreno.
     - **Food & Cuisine:** Data table (e.g., regional dishes, ingredients, or spice levels) and second featured image.
     - **Credits & References:** Detailed attribution lists organized by page.
   - Establish the site-wide header, navigation, main content area, and footer.
   - Define responsive breakpoints for 320px, tablet, and 1920px layouts.
   - Reuse one visual system across all pages while giving each page a clear purpose.

3. **Set up the static project**
   - Create the four page files (`index.html`, `culture.html`, `food.html`, `credits.html`) and shared stylesheet in the workspace.
   - Use relative file paths (e.g., `css/styles.css`, `images/photo.webp`) for all internal links, assets, and favicons so the site works reliably both locally and when hosted on GitHub Pages.
   - Set up a favicon package that works across mobile, tablet, and desktop devices.
   - Reuse the same navigation and skip-to-content pattern on every page.

4. **Build semantic, accessible HTML**
   - Create four HTML pages:
     - a major attractions home page (`index.html`);
     - a culture and traditions page;
     - a food and cuisine page;
     - a credits/references page.
   - Include at least the following HTML features across the site:
     - one accessible HTML table with a header row and appropriate `scope` attributes;
     - at least two optimized images, each with explicit `width` and `height` attributes to prevent layout shifts and useful alternative text (or an empty `alt=""` attribute only when decorative);
     - one audio or video element with `controls`, `preload="metadata"`, and a caption/transcript or alternative information when applicable; set dimensions for video, but not audio unless needed for its visible player layout;
     - at least one `<blockquote>`;
     - one semantically correct, keyboard-accessible static contact-form demo with a `<fieldset>` and `<legend>` where appropriate, associated `<label>` elements, and a visibly disabled submit control; clearly state that it does not submit or send data;
     - a unique, descriptive SEO `<meta name="description">` tag on every page;
     - favicon links and favicon assets on every page using relative paths;
     - the same site navigation on every page, with working relative links to all four pages;
     - valid landmarks and a logical heading order.
   - Avoid templates or frameworks and write organized, well-indented semantic HTML.
   - Record the exact page(s) on which every external asset or quoted resource appears in the credits.

5. **Source and optimize licensed content**
   - Use Creative Commons licenses for all externally sourced text, images, audio, video, and other media wherever possible.
   - Verify the exact Creative Commons license and version (for example, CC BY 4.0 or CC BY-SA 4.0) and confirm it permits the intended use, publication, and any edits or format conversions; check attribution, share-alike, non-commercial, and no-derivatives terms.
   - Avoid assets with unclear permissions or restrictions incompatible with the project. Preserve required attribution, creator names, license names and versions, license links, and source links.
   - Do not use copyrighted assets unless their permissions explicitly allow the intended project use; prefer Creative Commons throughout.
   - Download or generate optimized local copies of images and media in web-friendly formats with appropriate browser and codec support when permitted.
   - Record source, creator, license, usage page, and link for each asset in the credits.
   - The culture page uses “Cuando la vida se va,” a bambuco excerpt credited to Alexander Cuesta-Moreno on Wikimedia Commons, under CC BY-SA 3.0; the site uses Wikimedia Commons’ MP3 transcode with the audio content unchanged.
   - Include the AI chat or AI resource used and its contribution to the project.
   - Credit each external text passage, image, audio/video, blockquote, and custom font separately and identify the exact page where it is used.
   - If original copy or assets are created for the project, identify them as original work and do not falsely describe them as Creative Commons or as third-party content.

6. **Implement the shared responsive design**
   - Code mobile first: begin with the default/base CSS for a narrow mobile viewport, then progressively enhance layouts with `min-width` media queries for tablet and desktop. Do not start with a desktop layout and shrink it down.
   - Create a mobile-first external stylesheet shared by all four pages.
   - Create or reuse a reset/normalize stylesheet only if needed, and keep the main responsive rules in the shared external stylesheet.
   - Use CSS Grid for a major layout at least once.
   - Use CSS Flexbox for a navigation, card, or control layout at least once.
   - Use at least one custom font loaded locally (with relative paths) or with an appropriate Creative Commons, open-font, or otherwise permitted web-font license.
   - Add visible keyboard focus styles and logical, non-ambiguous interactive states.
   - Ensure no horizontal overflow from 320px through at least 1920px.
   - Test both a 320px-wide viewport and a 1920px-wide viewport, plus intermediate tablet and mobile widths.
   - Verify the base styles work without relying on larger-screen media queries, then verify each wider breakpoint adds or adjusts layout as intended.

7. **Verify accessibility and performance**
   - Check that a visible-on-focus skip-to-content link appears before navigation on every page and bypasses the header correctly.
   - Check heading structure, landmarks, labels, link purpose, keyboard navigation, and visible focus.
   - Verify link hover and focus states preserve sufficient text/background contrast, including links on colored sections.
   - Verify image alternative text and dimensions, video dimensions where applicable, captions or transcripts where appropriate, form semantics and submission behavior, and control focus.
   - Test every internal link and confirm the navigation works on all pages.
   - Verify that images are reasonably compressed/resized and video/audio is suitable for web delivery.
   - Confirm the HTML has no template/framework leftovers and no broken local or external links.
   - Run responsive checks at mobile, tablet, and desktop widths.

8. **Validate and prepare publication handoff**
   - Use HTML and CSS validation tools and resolve reported quality or syntax issues.
   - Inspect the final four-page project with a local web server.
   - Confirm HTML and CSS validate or that every validation warning/error has been reviewed and resolved.
   - Prepare the complete source and concise instructions for the user to create a public GitHub repository, publish the project, and verify that it is viewable outside the local environment; the user will handle publication.

## Key Deliverables

- Four complete HTML pages (including `index.html` as the entry point)
- One shared external stylesheet plus any permitted reset/normalize stylesheet
- Local, optimized, properly licensed assets in web-friendly formats
- A favicon set/references covering mobile, tablet, and desktop
- A detailed credits page with per-asset page usage
- Complete source ready for the user to publish to a public GitHub repository, with publication instructions

## Validation Checklist

- [ ] Location and content scope are defined.
- [ ] One of the three location pages is saved as `index.html` as the site's main entry point.
- [ ] All four pages exist and share navigation and favicon assets.
- [ ] All internal links, images, fonts, and favicons use relative file paths.
- [ ] Navigation links to all four pages from all four pages.
- [ ] Each page has a unique description meta tag.
- [ ] HTML includes the table, two images, media element, blockquote, and contact form mapped across the pages.
- [ ] The table, images, media, blockquote, and form meet semantic and accessibility requirements; the static demo form clearly states that it does not submit or send data.
- [ ] Images and video have explicit dimensions where applicable; audio has dimensions only if required by the visible player layout. Media uses optimized formats with suitable browser and codec support.
- [ ] Grid and Flexbox are both used in CSS.
- [ ] One custom font is included.
- [ ] The layout is mobile-first and responsive from 320px to 1920px.
- [ ] Skip link, keyboard navigation, link hover/focus contrast, labels, and semantic structure work.
- [ ] Media is optimized and all third-party and AI sources are credited with usage pages.
- [ ] Project passes HTML/CSS validation and is ready for the user's GitHub publication and public-access checks.
