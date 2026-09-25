# RigLogic

**Built for Better Controls. Mostly.**

This repository is the public home for RigLogic: its website, public documentation, releases, and issue tracking.

The Windows application itself is still being polished and its application source is intentionally not published here yet. This repository contains only public-facing material.

## Website

The current marketing site lives in `website/`.

It is a static site designed for GitHub Pages—no server, database, account system, or backend is required. During pre-release the site remains marked `noindex,nofollow`, and the download controls point visitors toward GitHub Releases without pretending a public player build already exists.

A Pages workflow is included under `.github/workflows/pages.yml`. Once GitHub Pages is enabled for this repository with **GitHub Actions** as the source, changes to `website/` on `main` can deploy automatically.

## Public repository structure

```
RigLogic/
├── website/                 # Static marketing website
├── docs/                    # Public-facing documentation
├── .github/
│   └── workflows/
│       └── pages.yml        # GitHub Pages deployment
└── README.md
```

Public Windows releases will eventually live under **GitHub Releases** in this repository. Application source, private build infrastructure, and unreleased implementation details stay outside this repo.

## Status

RigLogic is still in active pre-release development. Website copy, screenshots, compatibility notes, and download links may change before the first public release.

The current site uses neutral illustrated example setups instead of a personal controller profile. Fresh native application screenshots can replace those illustrations before launch.
