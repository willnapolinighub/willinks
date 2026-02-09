# Contributing to Will Napolini Portfolio

First off, thank you for considering contributing to this project! 🎉

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Style Guidelines](#style-guidelines)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)

## Code of Conduct

### Our Pledge
We are committed to providing a welcoming and inclusive environment for everyone, regardless of experience level, gender identity, sexual orientation, disability, personal appearance, body size, race, ethnicity, age, religion, or nationality.

### Expected Behavior
- Be respectful and considerate
- Welcome newcomers and help them get started
- Focus on what's best for the community
- Show empathy towards others

### Unacceptable Behavior
- Harassment, trolling, or insulting comments
- Personal or political attacks
- Publishing others' private information
- Any conduct that could be considered inappropriate in a professional setting

## How Can I Contribute?

### Reporting Bugs 🐛

Before creating a bug report, please check existing issues to avoid duplicates.

**Great bug reports include:**
- A clear, descriptive title
- Steps to reproduce the issue
- Expected behavior vs actual behavior
- Screenshots (if applicable)
- Browser and version information
- Any error messages from the console

**Template:**
```markdown
**Bug Description**
A clear description of what the bug is.

**To Reproduce**
Steps to reproduce:
1. Go to '...'
2. Click on '...'
3. Scroll down to '...'
4. See error

**Expected Behavior**
What you expected to happen.

**Screenshots**
If applicable, add screenshots.

**Environment:**
- Browser: [e.g. Chrome 120]
- OS: [e.g. macOS 14]
- Device: [e.g. iPhone 13]
```

### Suggesting Enhancements 💡

Enhancement suggestions are tracked as GitHub issues.

**Great enhancement suggestions include:**
- A clear, descriptive title
- Detailed description of the proposed functionality
- Explanation of why this would be useful
- Examples of how it would work
- Mockups or wireframes (if applicable)

**Examples of good enhancements:**
- "Add smooth scroll behavior to anchor links"
- "Include a 'Copy Email' button with clipboard API"
- "Add animation to theme transition"

### Your First Code Contribution 🚀

Unsure where to begin? Look for issues labeled:
- `good first issue` - Small, beginner-friendly changes
- `help wanted` - Issues that need attention
- `documentation` - Improvements to docs

### Areas to Contribute

**Design & UI:**
- New theme color schemes
- Animation improvements
- Layout enhancements
- Mobile responsiveness fixes

**Functionality:**
- Performance optimizations
- Accessibility improvements
- Browser compatibility fixes
- New interactive features

**Documentation:**
- README improvements
- Code comments
- Tutorial creation
- Translation to other languages

**Testing:**
- Cross-browser testing
- Mobile device testing
- Accessibility audits
- Performance profiling

## Development Setup

### Prerequisites
- A modern web browser
- A code editor (VS Code recommended)
- Basic knowledge of HTML, CSS, and JavaScript
- Git for version control

### Local Setup

1. **Fork the repository**
   - Click the "Fork" button at the top right of the GitHub page

2. **Clone your fork**
```bash
git clone https://github.com/YOUR_USERNAME/portfolio.git
cd portfolio
```

3. **Create a branch**
```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/bug-description
```

4. **Open in browser**
```bash
# Simply open index.html in your browser
# No build process needed!
```

5. **Make your changes**
   - Edit the code
   - Test in multiple browsers
   - Check responsive design

6. **Test your changes**
   - Open browser DevTools (F12)
   - Check Console for errors
   - Test all interactive features
   - Verify on mobile viewport

### Testing Checklist

Before submitting your PR, verify:

- [ ] Code works in Chrome, Firefox, and Safari
- [ ] Mobile responsive (test at 375px width)
- [ ] No JavaScript console errors
- [ ] All links work correctly
- [ ] Theme switching functions properly
- [ ] localStorage persists correctly
- [ ] Animations are smooth
- [ ] Accessibility maintained (tab navigation, ARIA labels)
- [ ] Code follows style guidelines

## Style Guidelines

### HTML

```html
<!-- ✅ Good: Semantic, accessible, clean -->
<a href="https://example.com" 
   class="glass-base rounded-xl p-4" 
   aria-label="Visit Example"
   target="_blank"
   rel="noopener noreferrer">
  <i class="fab fa-example"></i>
</a>

<!-- ❌ Bad: Missing attributes, unclear -->
<div onclick="goToSite()">
  <i class="fa fa-example"></i>
</div>
```

**Rules:**
- Use semantic HTML5 elements
- Include ARIA labels for accessibility
- Add `rel="noopener noreferrer"` for external links
- Keep structure logical and indented (2 spaces)

### CSS

```css
/* ✅ Good: Organized, commented, uses variables */
.custom-component {
  /* Layout */
  display: flex;
  align-items: center;
  
  /* Visual */
  background: var(--glass-bg);
  border-radius: 12px;
  
  /* Animation */
  transition: var(--transition);
}

/* ❌ Bad: Disorganized, no grouping */
.custom-component {
  border-radius: 12px;
  display: flex;
  background: rgba(255,255,255,0.08);
  transition: all 0.3s ease;
  align-items: center;
}
```

**Rules:**
- Use CSS custom properties (variables) for reusability
- Group related properties (layout, visual, animation)
- Add comments for complex sections
- Prefer `rem` units for scalability
- Use meaningful class names

### JavaScript

```javascript
// ✅ Good: Clear, commented, error handling
/**
 * Applies a theme to the page
 * @param {number} index - Theme index from themes array
 */
function applyTheme(index) {
  if (index < 0 || index >= themes.length) {
    console.error('Invalid theme index');
    return;
  }
  
  const theme = themes[index];
  document.body.className = theme.classes;
  localStorage.setItem('themeIndex', index);
}

// ❌ Bad: Unclear, no validation
function apply(i) {
  document.body.className = themes[i].classes;
  localStorage.setItem('themeIndex', i);
}
```

**Rules:**
- Use descriptive variable and function names
- Add JSDoc comments for functions
- Include error handling
- Use `const` and `let` (avoid `var`)
- Follow camelCase naming convention
- Keep functions focused (single responsibility)

### Naming Conventions

| Type | Convention | Example |
|------|-----------|---------|
| CSS Classes | kebab-case | `.theme-switcher` |
| JavaScript Variables | camelCase | `currentThemeIndex` |
| JavaScript Functions | camelCase | `applyTheme()` |
| Constants | UPPER_SNAKE | `MAX_THEMES` |
| IDs | camelCase | `themeSwitcher` |

## Commit Guidelines

### Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types
- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, no logic change)
- **refactor**: Code refactoring
- **perf**: Performance improvements
- **test**: Adding or updating tests
- **chore**: Maintenance tasks

### Examples

```bash
# Good commits
git commit -m "feat(themes): add sunset gradient theme"
git commit -m "fix(mobile): resolve overflow issue on small screens"
git commit -m "docs(readme): add browser compatibility section"
git commit -m "style(css): improve glassmorphism contrast"
git commit -m "perf(js): optimize theme switching animation"

# Bad commits
git commit -m "fixed stuff"
git commit -m "updates"
git commit -m "WIP"
```

### Commit Best Practices

- Write in present tense ("add feature" not "added feature")
- Keep subject line under 50 characters
- Capitalize subject line
- Don't end subject line with a period
- Use body to explain *what* and *why*, not *how*
- Reference issues in footer (`Fixes #123`)

## Pull Request Process

### Before Submitting

1. **Update documentation** if you've changed functionality
2. **Test thoroughly** across multiple browsers
3. **Ensure code follows style guidelines**
4. **Check for console errors**
5. **Update README** if adding features

### PR Template

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Performance improvement
- [ ] Refactoring

## Testing
Describe testing performed:
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] Mobile (iOS/Android)

## Screenshots
If applicable, add screenshots

## Checklist
- [ ] Code follows style guidelines
- [ ] Self-reviewed code
- [ ] Commented complex code
- [ ] Updated documentation
- [ ] No console warnings/errors
- [ ] Tested on multiple browsers
- [ ] Mobile responsive

## Related Issues
Fixes #(issue number)
```

### Review Process

1. **Automated checks** will run (if configured)
2. **Maintainer review** within 48-72 hours
3. **Feedback addressed** through discussion
4. **Approval and merge** when ready

### After Your PR is Merged

- Delete your feature branch
- Update your local repository
- Celebrate! 🎉 You've contributed to open source!

## Getting Help

### Resources
- **Documentation**: Read DOCUMENTATION.md for technical details
- **Issues**: Check existing issues and discussions
- **Contact**: Reach out via GitHub issues or Twitter

### Questions?

Don't hesitate to ask! Create an issue with the `question` label or join discussions.

Remember:
- There are no dumb questions
- Everyone was a beginner once
- The community is here to help

## Recognition

Contributors will be:
- Listed in the README
- Credited in release notes
- Thanked publicly on social media

Thank you for making this project better! 🚀

---

**Happy Contributing!**

*Last Updated: February 9, 2025*
