# Academic Personal Website Build Checklist

This document turns the implementation plan into a concrete build checklist for an academic personal website modeled after [jakubjdolezal.github.io](https://jakubjdolezal.github.io/) and intended for deployment on GitHub Pages.

## 1. Project Goal

Build a clean academic personal website that:

- introduces you and your research clearly
- highlights publications, projects, talks, and teaching
- is easy to update using Markdown
- is hosted publicly on GitHub Pages
- can later support a custom domain and small design refinements

## 2. Recommended Stack

Use:

- GitHub Pages for hosting
- Jekyll for static site generation
- the [Academic Pages](https://github.com/academicpages/academicpages.github.io) template as the starting point

Why this stack:

- it closely matches the reference site
- it is widely used for academic portfolios
- most content can be added as Markdown files rather than custom code
- GitHub Pages supports the workflow well

## 3. Success Criteria For Version 1

Version 1 is complete when:

- the site is live at `https://<github-username>.github.io/`
- the homepage clearly states your name, role, affiliation, and research focus
- your CV is downloadable
- publications are listed in a clean and credible format
- the site works well on mobile and desktop
- the navigation is simple and complete
- all major profile links work
- the site is easy to update without deep theme changes

## 4. Scope For Version 1

Include these pages or sections:

- Home
- Research or About
- Publications
- CV
- Projects or Portfolio
- Talks
- Teaching
- Contact

Optional for version 1:

- News updates
- Blog posts
- Awards
- Service
- Students or mentoring

## 5. Phase 0: Planning And Decisions

### Checklist

- [ ] Confirm the site audience:
  - [ ] faculty hiring committees
  - [ ] PhD or internship applications
  - [ ] collaborators
  - [ ] general academic visibility
- [ ] Decide whether the tone should be more research-focused, teaching-focused, or mixed
- [ ] Confirm the primary call to action:
  - [ ] read publications
  - [ ] download CV
  - [ ] contact for collaboration
  - [ ] browse projects
- [ ] Decide whether to use:
  - [ ] GitHub username site: `username.github.io`
  - [ ] project site under another repo
- [ ] Decide whether a custom domain is needed for launch or later
- [ ] Decide whether the site should be minimal now or include extra sections at launch

### Deliverable

A clear statement of the site purpose and initial page list.

## 6. Phase 1: Content Collection

Gather all materials before template customization.

### Identity

- [ ] Full name
- [ ] Preferred professional title
- [ ] Current position
- [ ] Institution and department
- [ ] City and country
- [ ] Professional email address
- [ ] Short bio, one paragraph version
- [ ] Longer bio, two to four paragraphs if needed

### Research Profile

- [ ] Three to six research interest keywords
- [ ] One plain-language research summary
- [ ] One more technical research summary
- [ ] Current projects summary
- [ ] Lab or group affiliation links

### Publications

- [ ] Complete publication list
- [ ] Citation data for each item
- [ ] Publication status labels where relevant:
  - [ ] published
  - [ ] accepted
  - [ ] preprint
  - [ ] under review
- [ ] DOI links
- [ ] PDF links where allowed
- [ ] code links
- [ ] project page links
- [ ] abstracts or short descriptions for selected papers

### CV And Documents

- [ ] Up-to-date CV in PDF
- [ ] one-page résumé if relevant
- [ ] research statement if you want it public
- [ ] teaching statement if you want it public

### External Links

- [ ] Google Scholar
- [ ] ORCID
- [ ] GitHub
- [ ] LinkedIn
- [ ] Semantic Scholar or DBLP if relevant
- [ ] institutional profile page

### Media And Assets

- [ ] Professional headshot
- [ ] Optional banner or supporting visual
- [ ] Favicon
- [ ] Any diagrams, screenshots, or project thumbnails

### Teaching And Talks

- [ ] Course list
- [ ] teaching role for each course
- [ ] lecture slides if public
- [ ] invited talks
- [ ] conference talks
- [ ] workshop tutorials

### Deliverable

A complete content folder on your machine with text, PDFs, images, and links ready for insertion.

## 7. Phase 2: Repository Setup

### Checklist

- [ ] Create a GitHub account if needed
- [ ] Create a repository named `username.github.io`
- [ ] Make the repository public
- [ ] Add a short repository description
- [ ] Decide whether to start from:
  - [ ] GitHub template import
  - [ ] local clone of the Academic Pages repo
- [ ] Add a `README.md` describing the purpose of the site repo

### Recommended Approach

Use the Academic Pages template repository as the base and then customize the content and styling locally.

### Deliverable

A GitHub repository exists and is ready for local development.

## 8. Phase 3: Local Development Environment

### Checklist

- [ ] Install Git
- [ ] Install Ruby and Bundler
- [ ] Clone the website repository locally
- [ ] Install Jekyll dependencies
- [ ] Run the site locally with a development server
- [ ] Confirm the default template builds successfully before editing content

### Verification

- [ ] local homepage loads
- [ ] no critical build errors
- [ ] navigation renders
- [ ] asset paths work locally

### Deliverable

A local working copy of the site that can be previewed before deployment.

## 9. Phase 4: Information Architecture

### Checklist

- [ ] Review the default navigation and remove unnecessary pages
- [ ] Finalize the main menu order
- [ ] Decide which page should act as:
  - [ ] homepage introduction
  - [ ] research overview
  - [ ] publication archive
  - [ ] project showcase
- [ ] Decide whether to expose blog or news in the first release
- [ ] Keep the top navigation concise

### Recommended Navigation For V1

1. Home
2. Publications
3. Projects
4. Talks
5. Teaching
6. CV
7. Contact

### Deliverable

A final sitemap and page order.

## 10. Phase 5: Site Configuration

Primary file area:

- `_config.yml`

### Checklist

- [ ] Set site title
- [ ] Set your full name
- [ ] Set site URL
- [ ] Set base URL correctly
- [ ] Set author metadata
- [ ] Add affiliation
- [ ] Add social links
- [ ] Set navigation labels
- [ ] Confirm timezone and locale if relevant
- [ ] Configure analytics only if desired

### Quality Checks

- [ ] page titles are correct
- [ ] social links are valid
- [ ] no placeholder author data remains
- [ ] no template demo text remains

### Deliverable

Global site metadata is personalized and production ready.

## 11. Phase 6: Homepage Build

The homepage should answer three questions immediately:

- Who are you?
- What do you work on?
- Where can people find your work or contact you?

### Checklist

- [ ] Add your name and role prominently
- [ ] Add a professional headshot
- [ ] Add a short introduction paragraph
- [ ] Add research interests
- [ ] Add quick links to:
  - [ ] CV
  - [ ] Google Scholar
  - [ ] GitHub
  - [ ] email
- [ ] Add a selected publications section
- [ ] Add a short featured projects section if useful
- [ ] Add current affiliation and position
- [ ] Remove all placeholder text

### Recommended Content Blocks

- Intro
- Current role and affiliation
- Research interests
- Selected papers
- Featured project or two
- Contact or collaboration note

### Deliverable

A homepage that looks credible, personal, and immediately informative.

## 12. Phase 7: Publications

Academic Pages supports publication entries well, so this is a core part of the build.

### Checklist

- [ ] Choose the citation format style
- [ ] Add all core publications first
- [ ] Mark accepted or preprint items clearly
- [ ] Add links for PDF, DOI, code, and project pages
- [ ] Add abstracts for major papers if useful
- [ ] Highlight selected papers on the homepage
- [ ] Check author ordering and venue names carefully

### Quality Checks

- [ ] citations are consistent
- [ ] links resolve correctly
- [ ] PDFs open
- [ ] venue names are standardized
- [ ] dates are correct

### Deliverable

A complete, trustworthy publications section.

## 13. Phase 8: Projects, Talks, And Teaching

### Projects

- [ ] Add projects that strengthen your academic profile
- [ ] Prefer research software, demos, datasets, or prototypes
- [ ] Keep each entry concise
- [ ] Link to GitHub repos or demos where possible

### Talks

- [ ] Add invited talks
- [ ] Add conference presentations
- [ ] Add workshop tutorials
- [ ] Link slides or recordings if public

### Teaching

- [ ] List courses taught or assisted
- [ ] Clarify role for each course
- [ ] Add links to syllabi or notes if useful

### Deliverable

Supporting sections that broaden the site beyond the CV.

## 14. Phase 9: CV And Contact

### CV

- [ ] Upload CV PDF
- [ ] Add a visible download link in navigation or homepage
- [ ] Check the file opens correctly on mobile and desktop
- [ ] Update the file name to something professional and stable

### Contact

- [ ] Add email
- [ ] Add institutional affiliation
- [ ] Add relevant external profiles
- [ ] Decide whether to include office address or not
- [ ] Avoid publishing personal contact details unnecessarily

### Deliverable

Visitors can quickly download your CV and reach you professionally.

## 15. Phase 10: Design And Branding

Do enough customization to make the site feel personal while staying professional.

### Checklist

- [ ] Replace stock images and placeholders
- [ ] Adjust colors if desired
- [ ] Check typography readability
- [ ] Make spacing and headings consistent
- [ ] Ensure the homepage feels personal rather than template-like
- [ ] Add a favicon
- [ ] Review mobile spacing and image scaling

### Design Guidelines

- prioritize readability over novelty
- keep visual hierarchy strong
- avoid overcrowding the homepage
- make important links easy to find
- keep the design calm and academic

### Deliverable

A site that looks polished and personalized rather than copied directly from a template.

## 16. Phase 11: Testing And Quality Assurance

### Functional Checks

- [ ] all pages load
- [ ] all navigation links work
- [ ] publication links work
- [ ] PDF links work
- [ ] external profile links work
- [ ] no broken images

### Content Checks

- [ ] no placeholder text remains
- [ ] names, affiliations, and dates are correct
- [ ] grammar and spelling are clean
- [ ] publication metadata is consistent

### Responsive Checks

- [ ] homepage works on mobile
- [ ] navigation works on mobile
- [ ] publication pages remain readable on small screens
- [ ] CV links are easy to tap on mobile

### Technical Checks

- [ ] site builds locally without errors
- [ ] no missing assets
- [ ] no console-breaking issues if browser tools are checked

### Deliverable

A launch-ready version with no obvious content or navigation issues.

## 17. Phase 12: GitHub Pages Deployment

### Checklist

- [ ] push the site code to GitHub
- [ ] enable GitHub Pages for the repository
- [ ] confirm the publishing source
- [ ] wait for the first successful deployment
- [ ] open the live URL
- [ ] verify that assets load correctly on the live site

### Post-Deploy Checks

- [ ] homepage renders correctly
- [ ] internal links work on the live domain
- [ ] PDFs download from the live domain
- [ ] no base URL issues

### Deliverable

A public live website hosted on GitHub Pages.

## 18. Phase 13: Optional Launch Enhancements

These can happen after version 1 is live.

### Optional Upgrades

- [ ] add a custom domain
- [ ] add Google Analytics or Plausible
- [ ] improve SEO metadata
- [ ] add Open Graph preview images
- [ ] add a 404 page
- [ ] add a news or updates section
- [ ] add a blog
- [ ] add a publications import workflow if needed

### Deliverable

A more polished version 1.1 without blocking the main launch.

## 19. Suggested Timeline

### Day 1

- [ ] finalize scope
- [ ] collect identity materials
- [ ] create repository

### Day 2

- [ ] set up the template locally
- [ ] configure site metadata
- [ ] build the homepage draft

### Day 3

- [ ] add publications
- [ ] add CV and profile links
- [ ] add talks, projects, and teaching

### Day 4

- [ ] polish styling
- [ ] run QA checks
- [ ] deploy to GitHub Pages

### Day 5

- [ ] review the live site
- [ ] fix post-launch issues
- [ ] consider custom domain and analytics

## 20. Risks And Common Mistakes

- [ ] choosing a template but leaving too much demo content in place
- [ ] publishing with broken social or PDF links
- [ ] overloading the homepage with too much text
- [ ] inconsistent publication formatting
- [ ] forgetting mobile layout checks
- [ ] misconfiguring GitHub Pages base URL settings
- [ ] delaying launch for nonessential design tweaks

## 21. Definition Of Done Checklist

- [ ] live GitHub Pages URL works
- [ ] homepage clearly introduces you
- [ ] headshot and core links are present
- [ ] CV is downloadable
- [ ] publications are complete and accurate
- [ ] projects, talks, and teaching are included if in scope
- [ ] navigation is clean and easy to use
- [ ] mobile and desktop views both work
- [ ] no placeholder content remains

## 22. Recommended Next Step

Once this checklist is approved, the next implementation step should be:

1. create the GitHub repository
2. pull in the Academic Pages template
3. configure the global site metadata
4. replace template homepage content with your own profile information

