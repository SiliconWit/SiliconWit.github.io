# Personal Website - Development Notes

Professional website for research, education, and product development activities.

## Content Updates

### Adding Timeline Milestones

To add new career milestones or position changes:

1. Open `index.html`
2. Locate the `timelineData` array (around line 1099)
3. Add a new object at the beginning of the array (most recent first)

Example structure:
```javascript
{
    year: "Year Range",
    title: "Position Title",
    institution: "Institution Name", 
    description: "Brief description of role and responsibilities.",
    achievementTitle: "Section Title",
    achievements: [
        {
            year: "YYYY",
            text: "Action/Event",
            link: "",
            title: "",
            journal: ""
        },
        {
            year: "YYYY",
            text: "Published",
            link: "https://doi.org/10.xxxx/xxxxx",
            title: "Paper title",
            journal: "in Journal Name"
        }
    ]
},
```

### Adding New Publications

For new papers, just add them to the appropriate milestone's `achievements` array:

```javascript
{
    year: "2025",
    text: "Published",
    link: "https://doi.org/10.xxxx/xxxxx",
    title: "Paper title here",
    journal: "in Journal Name"
}
```

### Updating Core Areas

To modify focus areas, update the "Core Focus Areas" section around line 898. Each area contains:
- Description
- Highlights list (formatted with `→` bullets)

### File Structure

```
SamMachariaPhD.github.io/
├── index.html          # Main website file
├── assets/
│   └── img/
│       ├── favicon.ico  # Site icon
│       ├── logo.png     # Header logo
│       └── demopic/     # Background images
│           ├── motorProtein.jpg
│           └── windEnergy.jpg
└── README.md           # Development notes
```

## Technical Implementation

### Design Approach
- Responsive layout for desktop, tablet, mobile
- Timeline adapts to screen size
- Navigation adjusts for small screens

### Automated Features
- Copyright year updates automatically (2010 - current year)
- Smooth scrolling navigation
- Scroll progress indicator
- Content fade-in animations

### External Links Organization
Academic and professional profiles categorized as:
- Academic: ORCID, Google Scholar, ResearchGate
- Technical: GitHub, Stack Overflow, ACM
- Professional: EBK, IEK registrations  
- Platform: SiliconWit, Goodreads, JOSS reviewer

## Architecture

### Technology Choices
- Single HTML file with embedded CSS and JavaScript
- No external frameworks
- CSS Grid/Flexbox for layouts
- Vanilla JavaScript for interactions

### Color Scheme
- Primary: Blue gradient (#667eea to #764ba2)
- Research: Blue-cyan gradient
- Education: Green-teal gradient  
- Product: Pink-yellow gradient

### Mobile-First Responsive Breakpoints
- Desktop: > 768px (2-column timeline)
- Tablet: 481-768px (single column, larger text)
- Mobile: < 480px (compact layout)

## Potential Additions

### Possible Future Features
- [ ] Technical blog section
- [ ] Research visualization components
- [ ] Student supervision information
- [ ] Course materials access
- [ ] Contact form integration

### Current Optimizations
- Single file architecture
- Optimized image assets
- Minimal JavaScript usage
- Clean CSS implementation
- Efficient font loading (Inter)

## Maintenance

### Regular Updates
- [ ] Add publications with DOI links
- [ ] Update timeline with career changes
- [ ] Review biographical information
- [ ] Verify external link functionality

### Occasional Updates
- [ ] Update profile photo
- [ ] Add professional registrations
- [ ] Update platform links
- [ ] Review collaboration information

## Version Control

### Backup Approach
- Repository serves as primary backup
- All content under version control
- GitHub Pages serves from main branch
- No additional hosting dependencies

### Recovery Process
If issues arise:
1. Review commit history: `git log --oneline`
2. Revert to stable version: `git reset --hard <commit-hash>`
3. Force push if necessary: `git push --force`

## Contact Methods

Footer links include:
- ORCID (primary academic profile)
- SiliconWit (collaborative platform)
- Google Scholar (publication index)
- GitHub (project repository)

## Implementation Notes

### Design Decisions
- Single-file approach for maintainability
- Timeline data structure for easy updates
- Neutral color scheme
- Mobile-responsive design

### Technical Considerations
- Direct publication links preferred over intermediary pages
- Timeline entries include specific dates and achievements
- Three-pillar focus (Research, Education, Product Development)
- Collaborative innovation emphasis for SiliconWit

### Development Guidelines
- Test mobile compatibility after changes
- Use DOI links for publication references
- Maintain ORCID as primary academic identifier
- Emphasize collaborative rather than commercial aspects

---

*Website: https://sammachariaphd.github.io/*