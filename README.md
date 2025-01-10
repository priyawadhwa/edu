<p align="center">
  <a href="https://edu.chainguard.dev" target="_blank"><img src="https://edu.chainguard.dev/logos/3d-linky.png" width="200" heght="auto"></a>
</p>
<h1 align="center">Chainguard Academy</h1>

<a href="https://chainguard.dev/" target="_blank"><img alt="Chainguard" src="https://img.shields.io/badge/Chainguard-4445E7.svg?style=for-the-badge&logo=Chainguard&logoColor=white"></a>

Our **mission** is to enable developers to build software efficiently and securely with Chainguard. Visit our website at 🔗 [edu.chainguard.dev](https://edu.chainguard.dev)

You can find the educational resource files in Markdown under the `content` directory.

## Development

This site is based on the [Doks Hugo theme](https://github.com/h-enk/doks). 

If you would like to develop this project, clone this repo and install dependencies with `npm`. 

```sh
npm install
```

To run a local version of this site, use npm to start it.

```sh
npm run start
```

You'll then navigate to `localhost:1313` within the web browser of your choice. 

## 📑 Contributing

If you identify something that is a major change, please file an [issue](https://github.com/chainguard-dev/edu/issues/new). If you identify a minor change like a typo that needs to be updated, or tech tooling that has a newer package, you are welcome to open a pull request for review from the team.

### Date Format

In each post's header, the date format should follow year-month-day as `YYYY-MM-DD`.

### Adding Graphic Images

Please reduce the image's file size before adding the image to this project to make page loadtimes faster and more accessible. You can use a tool such as [TinyPNG](https://tinypng.com/). 

If you are using images, it's best to bundle it together with the appropriate Markdown file. Create a directory with the name of the new page. Within the directory, create an `index.md` file and add the images within the directory as well.

In practice, this will look like the following, with images in place for both the `getting-started-enforce-github` directory and the `install-enforce-github` directory and the relevant tutorials:

```
├── chainguard
│   ├── _index.md
│   ├── enforce-github
│   │   ├── _index.md
│   │   ├── getting-started-enforce-github
│   │   │   ├── check.png
│   │   │   ├── index.md
│   │   │   ├── protected-branch.png
│   │   │   └── repo-access.png
│   │   └── install-enforce-github
│   │       ├── configure.png
│   │       ├── index.md
│   │       ├── permissions.png
│   │       └── user-select.png
```

Within the Markdown file, add images like so, with the alt text at the front:

```
![Protect branches with Chainguard Enforce](protected-branch.png)
```

Run a local development environment to ensure that your file structure is set up as intended.

### Adding Videos

Use a liquid tag within the Markdown to embed a YouTube video. For example, if you would like to link to the YouTube video located at [https://www.youtube.com/watch?v=rqIcDrg1XOs](https://www.youtube.com/watch?v=rqIcDrg1XOs), you can pull the string after `v=` and use the following liquid tag on its own line within Markdown.

```
{{< youtube rqIcDrg1XOs >}}
```

### Adding Tags

Tags are autogenerated when you add the following line to a Markdown file's front matter: 

`tags: ["Tag1", Tag2", etc]`

This line should appear between the `draft` line and the `images` line in the front matter.   

For example: 

```
...
draft: false
tags: ["Chainguard Images", "Overview", "Product"]
images: []
menu:
...
```
When applying tags, please make sure they conform to the working tag list below so that the tagging logic is consistent. If you'd like to add a new tag or suggest a tag revision, please submit a PR with a justification for the change. 

Tags are based on:
* _Content topics_ covered in the content, such as tools (Enforce, apko, etc), orgs/standards (OCI, SLSA, etc), and other relevant topics (SBOMs, etc).
* _Content types_ represented by the content, such as procedural, conceptual, interactive, troubleshooting, etc. 

You can review our current list of [Tags](https://edu.chainguard.dev/tags).