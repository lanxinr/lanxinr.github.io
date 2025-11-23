# IDE621 Knowledge Base

A static website showcasing learning theories knowledge base prepared by Zhen Li.

## Project Structure

```
lanxinr.github.io/
├── home/                    # Main homepage
│   ├── index.html          # Homepage with learning theories overview
│   ├── index.md            # Markdown version of homepage
│   └── images/             # Images and assets for homepage
├── behaviorism/            # Behaviorism theory page
│   ├── index.html
│   └── index.md
├── cognitivism/            # Cognitivism theory page
│   ├── index.html
│   └── index.md
├── social-learning/        # Social Learning Theory page
│   ├── index.html
│   └── index.md
├── about/                  # About page (personal introduction)
│   ├── index.html
│   └── index.md
├── case/                   # Case study page
│   ├── index.html
│   └── index.md
└── README.md              # This file
```

## Generation Rules

### Content Language
- **All content must be in English**
- All text, headings, descriptions, and documentation should be written in English
- Only proper nouns (names, places) may retain their original language

### File Naming Conventions
- Use lowercase with hyphens for file and directory names
- Example: `social-learning/`, `index.html`
- Image files should use descriptive names: `behaviorism-details.png`

### Markdown File Requirement
- **Every HTML page must have a corresponding Markdown file**
- Each `index.html` should have a corresponding `index.md` in the same directory
- Markdown files should contain the same content as HTML files (without styling)
- This ensures content can be easily edited, version-controlled, and converted to other formats
- Example structure:
  ```
  page-name/
    ├── index.html
    └── index.md
  ```

### HTML Structure Rules
1. **Consistent Navigation**
   - All pages must include the same navigation menu
   - Navigation links should use relative paths: `../home/`, `../behaviorism/`
   - Active page should have `class="active"` on the corresponding link

2. **Styling Consistency**
   - Use the same color scheme across all pages:
     - Primary: `#226e93` (blue)
     - Secondary: `#ff9900` (orange)
     - Background: `#ffffff` (white)
     - Text: `#212121` (dark gray)
   - Use consistent fonts:
     - Headings: `Lora, serif`
     - Body: `Gentium Basic, serif`

3. **Hero Section**
   - All pages should have a hero section with background image
   - Hero section height: 340px (desktop), 250px (mobile)
   - Title should be centered and use white color

4. **Main Content Container**
   - Max width: 1200px
   - Padding: 40px 24px
   - Center aligned with auto margins

5. **Responsive Design**
   - Mobile breakpoint: 768px
   - Small mobile breakpoint: 479px
   - All layouts should adapt to smaller screens

### Page-Specific Rules

#### Homepage (`home/index.html`)
- Must include:
  - Three theory cards in a grid layout
  - Theory details images in a grid
  - Comparison table of learning theories
  - PDF preview section (if applicable)
  - Reference section with citations

#### Theory Pages (`behaviorism/`, `cognitivism/`, `social-learning/`)
- Must include:
  - Page title matching the theory name
  - Subtitle: "Knowledge Base prepared by Zhen Li"
  - Infographics section with PDF links
  - Examples section with external links
  - Learning Scenario section
  - Observation Checklist section
  - Reflection section with detailed text

#### About Page (`about/index.html`)
- Must include:
  - Personal introduction
  - Education section
  - Research experience & publications
  - Conference papers
  - Teaching experience
  - Professional experience
  - Certifications
  - Honors & awards

### Image Rules
- All images should be placed in `home/images/` directory
- Use relative paths: `images/filename.png` or `../home/images/filename.png`
- Images should be optimized for web (reasonable file size)
- Alt text must be provided for all images

### PDF Handling
- PDF files should be placed in `home/images/` directory
- Use iframe for PDF preview with fallback to object tag
- Include proper error handling for browsers that don't support PDF preview

### Code Style
- Use 2-space indentation
- Use semantic HTML5 elements
- Include proper meta tags (charset, viewport)
- All CSS should be in `<style>` tags within `<head>`
- Use descriptive class names following BEM-like conventions

## Development

### Starting Local Server

Using Python 3:
```bash
cd /Users/xsh/works/lanxinr/lanxinr.github.io
python3 -m http.server 8000
```

Then visit: http://localhost:8000/home/

### File Organization
- Keep HTML files in their respective directories
- Shared images go in `home/images/`
- Each page should be self-contained with its own styles

## Content Guidelines

### Writing Style
- Use clear, academic English
- Maintain consistent terminology
- Use proper academic citation format
- Keep paragraphs concise and well-structured

### Links
- External links should open in new tab (`target="_blank"`)
- Internal links use relative paths
- All links should have descriptive text

### Accessibility
- Provide alt text for all images
- Use semantic HTML elements
- Ensure sufficient color contrast
- Maintain logical heading hierarchy (h1 → h2 → h3)

## Maintenance

### Adding New Pages
1. Create new directory with lowercase name
2. Add `index.html` following the structure of existing pages
3. **Create corresponding `index.md` file with the same content**
4. Update navigation menu on all pages
5. Ensure consistent styling

### Updating Content
- Always maintain English language requirement
- **Always update both HTML and Markdown versions** - they should contain the same content
- Test responsive design after changes
- Verify all links work correctly
- Markdown files serve as the source of truth for content editing

## Notes
- This is a static website, no build process required
- All content is served directly from HTML files
- Images and PDFs are served as static assets
