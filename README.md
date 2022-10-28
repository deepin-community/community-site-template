# Template for creating a deepin community site

## Usage

1. Fork this repo
2. On the forked repo main page, click "Settings"
3. Click "Pages" on the left side
4. On the "Build and deployment" section, select the "Source" to "GitHub Actions"
5. Push any content change to the repo

After that, your site will be there in a minute.

You can check the deployment status via the "Environments" section by clicking on "github-pages" at the sidebar of your repo's main page, and use the "View deployment" button on the newly-opend page to access the deployed website.

Feel free to make any change to this repo and the online website will be updated once you pushed your changes to your fork.

## Get it running locally

This site template is powered by [HUGO](https://gohugo.io/). You can install it via your system's package manager or via official release, and all the things you can learned from their official website can be applied to this template repo.

> **note**
> The `hugo` version included in deepin **v20** is a little outdated, if you are using deepin v20, please consider download `hugo` release via [GitHub](https://github.com/gohugoio/hugo/releases/) or other package manager like [`Nix`](https://nixos.org/).

Here is a gist about how to quickly get it up and running:

0. Ensure you `cd`-ed to this folder (that contains this README.md file)
1. Ensure HUGO is installed: `hugo version`
2. Start a local server: `hugo server` (by default the local site can be accessed via `http://localhost:1313/`)
3. Create a new blog post: `hugo new post/your-post-title.md` (new file will be created at `content/post/your-post-title.md`, please note it will be a *draft* post by default)
4. Start a local server that included all *draft* posts: `hugo server -D`
5. Quick browse all available commands: `hugo -h`

## Theme

This repo contains a theme called [up-business-theme](https://themes.gohugo.io/themes/up-business-theme/), the vendored revision is `5144bddd81373502200e43ba8fb7f62f33e2e075`. We don't include it as a git sub-module to ensure it's easy to get everything work as easy as possible.
