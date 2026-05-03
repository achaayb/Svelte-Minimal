# Svelte Minimal

Minimal Svelte + Vite boilerplate

## Tree

```console
$ tree
.
├── Dockerfile
├── index.html
├── LICENSE
├── package.json
├── package-lock.json
├── README.md
├── src
│   ├── App.svelte
│   └── main.js
└── vite.config.js

2 directories, 9 files
```

## Package

```json
{
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview"
  },
  "devDependencies": {
    "@sveltejs/vite-plugin-svelte": "^5.0.3",
    "svelte": "^5.19.0",
    "vite": "^6.0.7"
  }
}
```

## Build & Run
```bash
podman|docker build -t svelte-minimal .
podman|docker run -p 8080:80 svelte-minimal
```

## Dockerfile
Multi-stage:
- Node → build
- Nginx → serve `dist/`

## Ignore
Custom `.gitignore` + `.dockerignore`
