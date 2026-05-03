# Svelte Minimal

Minimal Svelte + Vite boilerplate

## Tree

```console
$ tree -la -I 'dist|node_modules|.git'
.
├── Dockerfile
├── .dockerignore
├── .gitignore
├── index.html
├── LICENSE
├── package.json
├── package-lock.json
├── README.md
├── src
│   ├── App.svelte
│   └── main.js
└── vite.config.js

2 directories, 11 files

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

## Shallow Clone
```bash
git clone --depth 1 https://github.com/achaayb/Svelte-Minimal <project-name>
```

## Build & Run
```bash
podman|docker build -t <image-name> .
podman|docker run -p 8080:80 <image-name>
```

## Dockerfile
Multi-stage:
- Node → build
- Nginx → serve `dist/`

## Ignore
Custom `.gitignore` + `.dockerignore`
