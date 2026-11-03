# Campus Eats — Lab 07 (Figma to Website)

A small, student-level responsive website for the Campus Eats university food concept. It uses plain HTML, CSS and JavaScript so it is easy to read and edit.

## Project sections

1. Navigation bar with mobile menu
2. Hero section with two call-to-action links
3. Three-card feature grid
4. Contact form and footer

## Responsive widths

- Desktop: 1440px layout target
- Tablet: 768px layout target
- Mobile: 375px layout target

The CSS uses a two-column hero and three-column card grid on desktop, a two-column card grid on tablet, and a single-column layout on mobile. No fixed absolute positioning is used for the main page layout.

## Run locally

No package installation is required.

1. Open this folder in VS Code.
2. Open `index.html` in a browser, or use the VS Code Live Server extension.
3. Resize the browser to 1440px, 768px and 375px to review the layout.

## Figma file

[Campus Eats — Lab 07 Figma file](https://www.figma.com/design/vebnyGPVNK1LmkvGEq29iw)

The file contains:
- `Design System`: color and spacing variables, typography styles, button variants, feature-card variants, navigation-link variants, and an SVG-exportable vector icon.
- `Website Layouts`: Desktop Website (1440px), Tablet Website (768px), and Mobile Website (375px) frames.

## Figma MCP setup in VS Code

A workspace configuration is included at `.vscode/mcp.json`.

1. Open this folder in VS Code.
2. Press `Ctrl + Shift + P`.
3. Search for **MCP: Open Workspace Folder Configuration** if you need to view/edit the MCP config.
4. The included config points to the recommended remote Figma MCP server: `https://mcp.figma.com/mcp`.
5. Save the file and click **Start** above the Figma server entry.
6. Sign in to Figma and allow access when prompted.
7. Open VS Code Agent mode and use the Figma MCP tools with the selected frame link.

Example prompt for your IDE agent:

> Inspect the selected Campus Eats frame. Extract design variables and create responsive semantic HTML5 and CSS. Use header, nav, main, section and footer landmarks. Keep the existing color tokens, use the 1440px, 768px and 375px breakpoints, and ensure that labels, keyboard focus states and image alt text are present.

Figma's current official guide recommends the remote endpoint. The current VS Code config uses `inputs`, `servers`, and `type: "http"`.

## Accessibility and interaction notes

- Uses semantic `header`, `nav`, `main`, `section`, `form` and `footer` elements.
- Each contact input has a visible `label` with a matching `for` and `id`.
- Decorative card icons have empty alt attributes; the main illustration has descriptive alt text.
- Links and controls have visible hover and keyboard focus states.
- The mobile menu has `aria-expanded` and `aria-controls` attributes.
- The contact form performs browser validation and displays a demo success message. It does not send or store messages because there is no backend.

## Publish to GitHub and deploy

This folder is ready to upload to a public GitHub repository. After pushing it, you can deploy the repository using a static host such as Vercel or GitHub Pages. No build command is needed; the site is static HTML/CSS/JS and the output directory is the project root.

Suggested repository name: `campus-eats-lab07`

Suggested Vercel settings:
- Framework preset: Other
- Build command: leave blank
- Output directory: `.` (project root)

## Important

The website is a front-end demonstration. The contact form does not submit to a server, and it does not process real food orders or payments.
"# figma__frontend" 
"# figma__frontend" 
