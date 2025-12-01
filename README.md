# Student Visual Portfolio Platform

A comprehensive, production-ready multi-format portfolio platform with in-browser content editing, full agile requirement coverage, and advanced collaboration features.

## Features

- **Multi-Content Management**: Projects, Presentations, Articles, Certifications, Code Snippets
- **Advanced Theming**: Minimalist, Corporate, Creative themes + custom accent color picker
- **User Authentication**: GitHub OAuth + Magic Links with role-based access
- **Project Collaboration**: Invite teammates, shared attribution, multi-portfolio linking
- **In-Browser Editor**: WYSIWYG editing with TipTap editor, auto-save, image upload
- **Project Duplication**: Clone existing projects with pre-filled forms
- **Real-time Sync**: Live collaboration with Supabase real-time subscriptions

## Tech Stack

- **Frontend**: Tailwind CSS 3.x, ES6+ modules, Anime.js animations
- **Editor**: TipTap rich text editor with markdown support
- **Backend**: Supabase (PostgreSQL + Realtime + Storage)
- **Authentication**: GitHub OAuth + Magic Links
- **Charts**: Plotly.js for skill visualizations
- **PDF**: PDF.js for presentation viewer
- **Syntax**: Prism.js with custom theme

## Quick Start

1. **Clone and Install**
   ```bash
   git clone <repository-url>
   cd student-portfolio-platform
   npm install
   ```

2. **Setup Supabase**
   - Create a new Supabase project at [supabase.com](https://supabase.com)
   - Copy the URL and anon key from Settings > API
   - Create tables using the schema in `supabase/schema.sql`
   - Enable Row Level Security (RLS) policies

3. **Configure Environment**
   ```bash
   cp .env.example .env
   # Edit .env with your Supabase credentials
   ```

4. **Run Development Server**
   ```bash
   npm run dev
   # Open http://localhost:3000
   ```

5. **Run Tests**
   ```bash
   npm run test
   npm run test:e2e
   ```

## Project Structure

```
src/
├── index.html          # Landing page with hero and featured projects
├── projects.html       # Full project management with editing
├── presentations.html  # PDF viewer for talks with editing
├── cv.html            # Vertical CV format with editable sections
├── docs.html          # Agile requirements documentation
├── css/
│   └── style.css      # Custom Tailwind plugins and styles
├── js/
│   ├── main.js        # Core functionality and auth
│   ├── projects.js    # Project CRUD and collaboration
│   ├── editor.js      # TipTap editor and auto-save
│   └── supabase.js    # Backend integration
└── data/
    ├── projects.json   # Sample project data
    └── presentations.json # Sample presentation data
```

## User Stories Implemented

1. **US-001**: Theme System - Dark/light toggle with predefined themes
2. **US-002**: Skill Tags - Interactive filtering and display
3. **US-003**: Consistent UI - Unified design system across all pages
4. **US-004**: Project Duplication - Clone projects with pre-filled forms
5. **US-005**: Team Collaboration - Invite teammates and share attribution

## Editing Features

- **Rich Text Editor**: TipTap with markdown support, images, code blocks
- **Auto-Save**: Drafts saved to localStorage every 30 seconds
- **Image Upload**: Drag-and-drop with client-side compression
- **Live Preview**: Side-by-side preview while editing
- **Collaboration**: Real-time editing with user presence indicators
- **Validation**: Frontend and backend validation with error handling

## Deployment

1. **GitHub Pages** (Recommended)
   ```bash
   npm run build
   npm run deploy
   ```

2. **Netlify**
   - Connect your GitHub repository
   - Set build command: `npm run build`
   - Set publish directory: `dist`

3. **Vercel**
   - Import from GitHub
   - Framework preset: Static
   - Build command: `npm run build`

## Development Commands

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run test         # Run unit tests
npm run test:e2e     # Run Cypress E2E tests
npm run lint         # Run ESLint
npm run format       # Format code with Prettier
```

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -am 'Add feature'`
4. Push to branch: `git push origin feature-name`
5. Submit a pull request

## License

MIT License - see LICENSE file for details