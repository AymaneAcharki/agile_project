# Portfolio Project Structure

## File Organization
```
C:\Users\Achar\Desktop\Kedge\MSc_2\Automne 2025\Agile PM\DRAFT/
├── index.html                        # Main portfolio landing page
├── projects.html                     # Projects, Code & Technical Work
├── about.html                        # About, CV & Skills
├── presentations.html                # NEW: presentations, slides, talks
├── articles.html                     # NEW: blog posts & publications
├── certifications.html               # NEW: certifications & education
├── main.js                           # Core JavaScript functionality
├── resources/                        # Media and asset folder
│   ├── hero-bg.jpg                   # Hero background image
│   ├── project-*.jpg                 # Project preview images
│   ├── profile.jpg                   # Professional headshot
│   ├── presentations/                # NEW: Presentation files (PDF)
│   │   ├── deck-*.pdf                # Presentation slides
│   │   └── thumbnails/               # Presentation thumbnails
│   ├── code-snippets/                # NEW: Code examples
│   │   ├── notebook-*.ipynb          # Jupyter notebooks
│   │   └── snippet-*.js/py           # Code files
│   ├── certs/                        # NEW: Certifications
│   │   ├── cert-*.pdf                # Certificate PDFs
│   │   └── cert-thumbnails/          # Certificate images
│   └── tech-icons/                   # Technology skill icons
├── data/                             # NEW: Data files
│   ├── projects.json                 # Projects data
│   ├── presentations.json            # NEW: Presentations data
│   ├── articles.json                 # NEW: Articles data
│   └── certifications.json           # NEW: Certifications data
├── design.md                         # Design system documentation
├── interaction.md                    # Interaction design specs
├── project-structure.md              # This file
└── README.md                         # NEW: Project documentation
```

## Page Breakdown

### index.html - Portfolio Landing
- **Hero Section**: Animated introduction with key highlights carousel
- **Content Preview**: Featured projects, presentations, articles
- **Skills Overview**: Interactive skill tag cloud with proficiency levels
- **Quick Contact**: Floating contact form and social links
- **Content Categories**: Direct access to projects/presentations/articles

### projects.html - Projects & Code Showcase
- **Filter Bar**: Multi-filter (technology, type, date, content type)
- **Content Type Tabs**: Projects | Code Examples | Notebooks | Technical Demos
- **Grid Layout**: Responsive masonry for all technical work
- **Project Details**: Expandable cards with code samples, demos, repositories
- **Search Function**: Real-time search through all technical content
- **Code Preview**: Syntax-highlighted code with copy functionality
- **Live Demos**: Embedded iframes or external links

### presentations.html - Presentations & Talks
- **Presentation Grid**: Cards for talks, slides, conference presentations
- **Filter by Context**: Academic, Professional, Conference, Workshop
- **Embed Viewer**: PDF viewer for presentations
- **Metadata**: Event, date, audience, language
- **Download Links**: PDF/PPTX download
- **Video Recordings**: Links to recorded talks (YouTube)

### articles.html - Publications & Writing
- **Article List**: Blog posts, technical articles, publications
- **Categories**: Tutorial, Opinion, Case Study, Research
- **Reading Time**: Estimated read time
- **Publication Date**: Chronological sorting
- **Tags**: Topics and technologies
- **External Links**: Dev.to, Medium, LinkedIn, Research journals

### certifications.html - Certifications & Education
- **Certification Grid**: Certificates, diplomas, badges
- **Categories**: Degree, Professional Cert, Online Course
- **Verification**: Links to verification pages
- **Skills Mapping**: Relation avec les compétences techniques
- **Expiration Dates**: For time-limited certifications
- **Issuing Organizations**: School, university, platforms

### about.html - About, CV & Experience
- **Professional Summary**: Background and expertise areas
- **Interactive CV**: Downloadable PDF with multiple formats
- **Technical Skills**: Comprehensive skill breakdown with visual indicators
- **Experience Timeline**: Professional experience with details
- **Education History**: Academic background
- **Contact Information**: Professional links and email

## Content Strategy

### Project Data Structure
Each project includes:
- Title, subtitle, and detailed description
- Technology stack (skill tags with versions)
- Project type (web app, mobile, CLI tool, library, etc.)
- Content type (full project, code snippet, notebook, demo)
- Completion date and duration
- Your role and team size
- Code repository link (GitHub, GitLab)
- Live demo URL (Netlify, Vercel, Heroku)
- Screenshots/previews (multiple images)
- Features list (bullet points)
- Challenges and solutions
- Code highlights (key snippets)
- Performance metrics

### Presentation Data Structure
Each presentation includes:
- Title and subtitle
- Event name and type (conference, workshop, class)
- Date and duration
- Description/abstract
- Topics covered (tags)
- Audience level (beginner, intermediate, advanced)
- Language
- Slide deck (PDF or external link)
- Thumbnail image
- Video recording (YouTube, Vimeo)
- Key takeaways

### Article Data Structure
Each article includes:
- Title and subtitle
- Publication date
- Reading time (minutes)
- Category (tutorial, case study, opinion, research)
- Summary/excerpt
- Full content or external link
- Tags (technologies, topics)
- Publication platform (own blog, Medium, Dev.to)
- Featured image
- Author (if co-authored)

### Certification Data Structure
Each certification includes:
- Title (degree or certification name)
- Issuing organization (school, university, platform)
- Date earned and expiration (if applicable)
- Credential ID and verification URL
- Skills learned
- Category (degree, professional cert, course)
- Certificate image/PDF
- Description of program
- Grade/honors (if relevant)

### Content Type Categories
- **Full Projects**: Applications complètes, web/mobile
- **Code Libraries**: Packages, modules, open source
- **Code Snippets**: Examples, patterns, utils
- **Jupyter Notebooks**: Data science, analysis, ML
- **Technical Demos**: Proofs of concept, experiments
- **Presentations**: Slides, talks, workshops
- **Articles**: Blog posts, tutorials, guides
- **Case Studies**: Analyses détaillées de projets

### Skill Categories
- **Frontend**: HTML, CSS, JavaScript, React, Vue, Angular, TypeScript
- **Backend**: Python, Node.js, Django, Flask, FastAPI, Express
- **Databases**: PostgreSQL, MongoDB, Redis, MySQL, SQLite
- **DevOps**: Git, Docker, AWS, CI/CD, Kubernetes, Vercel
- **Design**: UI/UX, Tailwind CSS, Figma, Responsive Design
- **Data Science**: Pandas, NumPy, Scikit-learn, Jupyter, Matplotlib
- **Mobile**: React Native, Flutter, Swift, Kotlin
- **Tools**: VS Code, Linux, Postman, Browser DevTools

## Multi-Format Content Support

### Code Display
- Syntax highlighting (Prism.js or highlight.js)
- Copy-to-clipboard button
- Line numbers
- Multiple files per project
- Diff views for changes

### Presentation Display
- PDF.js for in-browser viewing
- Thumbnail navigation
- Fullscreen mode
- Download button
- Print-friendly versions

### Article Display
- Markdown rendering
- Code blocks highlighting
- Responsive typography
- Reading progress indicator
- Social sharing

### Media Management
- Image optimization (WebP with fallbacks)
- Lazy loading for all media
- Responsive images (srcset)
- Video embedding (YouTube, Vimeo)
- Audio files (podcasts, recordings)