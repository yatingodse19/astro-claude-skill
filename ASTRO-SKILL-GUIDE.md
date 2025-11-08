# Astro Builder Skill - Usage Guide

## Overview

I've created a comprehensive Claude skill for building websites with Astro.build! This skill will help you (and any Claude instance) to:

1. **Automatically browse and select appropriate themes** from Astro's free themes collection
2. **Access Astro's complete documentation** when needed
3. **Follow best practices** for Astro development
4. **Get step-by-step guidance** for building different types of websites

## What's Included

The skill package (`astro-builder`) contains:

### 1. SKILL.md - Main Instructions
The comprehensive guide that tells Claude:
- When to use this skill (any Astro-related request)
- How to select appropriate themes based on project requirements
- Where to access Astro documentation
- Step-by-step workflows for different website types (blog, portfolio, docs, etc.)
- Best practices and troubleshooting tips

### 2. references/astro_docs.md - Core Documentation
A curated reference containing:
- Core Astro concepts (Islands Architecture, Zero JS by default)
- Project structure requirements
- Component syntax and patterns
- Routing and navigation
- Styling options (scoped styles, global styles, Tailwind)
- Image optimization
- Configuration examples
- Content collections
- Framework integrations (React, Vue, Svelte)

### 3. scripts/theme_analyzer.py - Theme Helper
A Python script that can:
- Fetch themes from Astro's official themes page
- Filter by technology (React, Vue, Svelte, etc.)
- Filter by price (free/paid)
- Suggest themes based on project type

## How It Works

When you mention building with Astro, the skill will automatically:

1. **Understand Your Requirements**
   - Ask clarifying questions about your website type
   - Identify needed features (blog, portfolio, docs, e-commerce, etc.)

2. **Browse and Recommend Themes**
   - Fetch free React-compatible themes from: https://astro.build/themes/1/?technology%5B%5D=react&price%5B%5D=free
   - Analyze themes based on your requirements
   - Recommend 2-3 best-matching options with explanations

3. **Access Documentation as Needed**
   - First, reference the built-in `astro_docs.md` for quick answers
   - For advanced topics, fetch full documentation from https://docs.astro.build/llms-full.txt
   - Provide code examples and patterns

4. **Guide Development**
   - Set up proper project structure
   - Create components following Astro best practices
   - Implement routing and pages
   - Add interactivity only where needed (Islands Architecture)
   - Optimize for performance

## Example Use Cases

### Building a Blog
**You say:** "I want to build a blog with Astro and React"

**The skill will:**
1. Fetch blog-oriented themes from Astro themes page
2. Recommend themes like astro-paper or similar
3. Reference component syntax from astro_docs.md
4. Guide you through:
   - Setting up the project structure
   - Creating blog post layouts
   - Building listing and detail pages
   - Adding React components for comments/interactions
   - Setting up RSS feeds

### Creating a Portfolio
**You say:** "Create a portfolio site for me using https://astro.build/"

**The skill will:**
1. Ask about what you want to showcase
2. Fetch portfolio themes
3. Recommend based on your field (developer, designer, etc.)
4. Help create:
   - Hero section
   - Projects grid
   - About page
   - Contact form
   - Smooth page transitions

### Documentation Site
**You say:** "I need a documentation site with search and dark mode"

**The skill will:**
1. Recommend Starlight (Astro's official docs framework)
2. Show setup commands
3. Configure:
   - Sidebar navigation
   - Built-in search (Pagefind)
   - Dark mode
   - i18n if needed

## Key Features

### 🎨 Smart Theme Selection
- Automatically browses Astro's themes page
- Filters by technology (React, Vue, Svelte) and price
- Provides detailed recommendations with reasons

### 📚 Comprehensive Documentation Access
- Built-in reference for quick answers
- Can fetch full Astro documentation when needed
- Covers all major Astro features and patterns

### 🚀 Best Practices Built-In
- Islands Architecture (static by default)
- Performance optimization
- Type safety with TypeScript
- Image optimization
- SEO-friendly patterns

### 🔧 Troubleshooting Support
- Common issues and solutions
- Error message explanations
- Configuration help

## Installation

To use this skill with Claude:

1. **Upload the skill file**: Use the `.skill` file I've created
2. **Enable it in your project**: The skill will be available for all conversations
3. **Start building**: Just mention Astro or say you want to build a website!

## Technical Details

### Project Structure Created
```
project/
├── src/
│   ├── components/     # Reusable Astro/framework components
│   ├── layouts/        # Page layouts
│   ├── pages/          # Routes (REQUIRED)
│   ├── content/        # Content collections (optional)
│   └── assets/         # Optimized images
├── public/             # Static assets
├── astro.config.mjs    # Configuration
├── package.json
└── tsconfig.json
```

### Supported Technologies
- ✅ Astro components (.astro)
- ✅ React (.jsx, .tsx)
- ✅ Vue (.vue)
- ✅ Svelte (.svelte)
- ✅ Solid.js
- ✅ Preact
- ✅ TypeScript
- ✅ Markdown/MDX

### Key Concepts Covered
- Islands Architecture
- Component composition
- File-based routing
- Content Collections
- View Transitions
- Image optimization
- SEO best practices
- Performance optimization

## Why This Skill is Powerful

1. **Saves Time**: No need to manually browse themes or search documentation
2. **Best Practices**: Follows Astro's recommended patterns automatically
3. **Type-Safe**: Encourages TypeScript usage with proper examples
4. **Performance-First**: Emphasizes Astro's strengths (zero JS by default)
5. **Comprehensive**: Covers everything from setup to deployment

## Next Steps

1. **Install the skill** in your Claude environment
2. **Try it out** with a simple request like "Help me build an Astro blog"
3. **Watch it work** as it fetches themes, references docs, and guides you through development

## Customization

The skill can be customized by:
- Adding more theme categories
- Including additional documentation references
- Adding project templates
- Including deployment guides for specific platforms

## Support

The skill includes:
- Troubleshooting section for common issues
- Links to official Astro resources
- Example workflows for different project types
- Best practices for performance and SEO

---

**Ready to build amazing websites with Astro? Just upload the skill and start coding!** 🚀
