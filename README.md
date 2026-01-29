# Personal Portfolio

A clean, minimal, text-first personal portfolio website built with Next.js 16, Tailwind CSS 4, and TypeScript.

## Features

- **Modern Stack**: Next.js App Router, Tailwind CSS, TypeScript
- **Academic Style**: Clean, left-aligned, high-readability design
- **SEO Optimized**: Meta tags, Open Graph, Twitter cards
- **Accessible**: Semantic HTML, ARIA labels, focus states
- **Mobile Responsive**: Works on all screen sizes
- **Fast**: Minimal dependencies, optimized fonts

## Structure

```
src/
├── app/
│   ├── globals.css      # Global styles and CSS variables
│   ├── layout.tsx       # Root layout with SEO metadata
│   └── page.tsx         # Main portfolio page
└── components/
    ├── Section.tsx      # Reusable section wrapper
    ├── Header.tsx       # Name, bio, and contact links
    ├── Footer.tsx       # Copyright and credits
    ├── ProjectCard.tsx  # Project display component
    ├── PublicationItem.tsx  # Publication listing
    ├── ExperienceItem.tsx   # Work experience entry
    └── index.ts         # Component exports
```

## Getting Started

### Prerequisites

- Node.js 18+
- npm, yarn, pnpm, or bun

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the portfolio.

### Build

```bash
npm run build
npm run start
```

## Customization

1. **Update personal info**: Edit `src/components/Header.tsx` with your name, bio, and links
2. **Add experience**: Modify the Experience section in `src/app/page.tsx`
3. **Add projects**: Add `ProjectCard` components in `src/app/page.tsx`
4. **Add publications**: Add `PublicationItem` components in `src/app/page.tsx`
5. **Update metadata**: Edit `src/app/layout.tsx` for SEO

## Colors

The portfolio uses a clean, minimal color palette:

- **Background**: White (`#ffffff`)
- **Text**: Dark gray (`#1a1a1a`)
- **Muted text**: Gray (`#6b7280`)
- **Accent/Links**: Blue (`#2563eb`)
- **Borders**: Light gray (`#e5e7eb`)

## Deployment

### Vercel (Recommended)

```bash
npx vercel
```

### Static Export

Add to `next.config.ts`:

```typescript
const nextConfig = {
  output: 'export',
};
```

Then build:

```bash
npm run build
```

## License

MIT License - feel free to use this template for your own portfolio.
