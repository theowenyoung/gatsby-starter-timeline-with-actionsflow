<p align="center">
  <a href="https://www.gatsbyjs.com">
    <img alt="Gatsby" src="https://www.gatsbyjs.com/Gatsby-Monogram.svg" width="60" />
  </a>
</p>
<h1 align="center">
  Starter for the Gatsby timeline blog theme with Actionsflow
</h1>

Quickly get started using the Gatsby timeline blog theme with [Actionsflow](https://github.com/actionsflow/actionsflow)! This starter creates a new Gatsby site that is preconfigured to work with [Actionsflow](https://github.com/actionsflow/actionsflow)!

## 🚀 Quick start

1.  **Create a Gatsby site.**

    Use the Gatsby CLI to create a new site, specifying the blog theme starter.

    ```shell
    # create a new Gatsby site using the blog theme starter
    gatsby new my-themed-blog https://github.com/gatsbyjs/gatsby-starter-timeline-with-actionsflow
    ```

1.  **Config actionsflow workflow**

    > Note, for saving github resource, I comment the `.github/workflows/actionsflow.yml` `schedule` event, you should uncomment that if you want to use Actionsflow at github.

    We have a twitter workflow in there, for local, you should create `.secrets` with the following configuration:

    ```ini
    TWITTER_CONSUMER_KEY=xx
    TWITTER_CONSUMER_SECRET=xx
    TWITTER_ACCESS_TOKEN=xx
    TWITTER_ACCESS_SECRET=xx
    ```

    For github, you should add these secrets at your repo settings.

    Learn more about this please see [here](https://actionsflow.github.io/docs/workflow/)

1.  **Start developing.**

    Navigate into your new site’s directory and start it up.

    ```shell
    cd my-themed-blog/
    npm run start
    ```

1.  **Open the code and start customizing!**

    Your site is now running at `http://localhost:8000`!

    To get started, check out the guide to [using the Gatsby blog theme starter](https://gatsbyjs.com/docs/themes/using-a-gatsby-theme), or the longer, [more detailed tutorial](https://gatsbyjs.com/tutorial/using-a-theme).

## 🧐 What's inside?

Here are the top-level files and directories you'll see in a site created using the blog theme starter:

```text
├── LICENSE
├── README.md
├── content
│   ├── assets
│   │   └── avatar.png
│   └── posts
│       ├── hello-world
│       │   ├── index.mdx
│       │   └── sunset-beach.jpg
│       └── my-second-post.mdx
├── data
│   └── tweets
│       ├── image-tweet.json
│       ├── quote.json
│       ├── retweet.json
│       └── tweet.json
├── gatsby-config.js
├── package-lock.json
├── package.json
├── src
│   ├── gatsby-plugin-theme-ui
│   │   └── index.js
│   └── gatsby-theme-timeline
│       └── components
│           └── bio-content.js
└── workflows
    └── sync-tweets.yml
```

1.  **`/content`**: A content folder holding assets that the theme expects to exist. This will vary from theme to theme -- this starter is set up to get you started with the blog theme, which expects an image asset for your avatar, and blog post content. Replace the avatar image file, delete the demo posts, and add your own!

1.  **`/data/tweets`**: A tweets raw JSON folder, Actionsflow will add your tweets to this folder automatically

1.  **`/workflows`**: Actionsflow workflows folder, learn more about this please see [here](https://actionsflow.github.io/docs/workflow/)

1.  **`/src`**: You will probably want to customize your site to personalize it. The files under `/src/gatsby-theme-timeline` _shadow_, or override, the files of the same name in the `gatsby-theme-timeline` package. To learn more about this, check out the [guide to getting started with using the blog theme starter](https://gatsbyjs.com/docs/themes/using-a-gatsby-theme).

1.  **`.gitignore`**: This file tells git which files it should not track / not maintain a version history for.

1.  **`.prettierrc`**: This file tells [Prettier](https://prettier.io/) which configuration it should use to lint files.

1.  **`gatsby-config.js`**: This is the main configuration file for a Gatsby site. This is where you can specify information about your site (metadata) like the site title and description, which Gatsby plugins you’d like to include, etc. When using themes, it's where you'll include the theme plugin, and any customization options the theme provides.

1.  **`LICENSE`**: This Gatsby starter is licensed under the 0BSD license. This means that you can see this file as a placeholder and replace it with your own license.

1.  **`package-lock.json`** (See `package.json` below, first). This is an automatically generated file based on the exact versions of your npm dependencies that were installed for your project. **(You won’t change this file directly).**

1.  **`package.json`**: A manifest file for Node.js projects, which includes things like metadata (the project’s name, author, etc). This manifest is how npm knows which packages to install for your project.

1.  **`README.md`**: A text file containing useful reference information about your project.

## 🎓 Learning Gatsby

Looking for more guidance? Full documentation for Gatsby lives [on the website](https://www.gatsbyjs.com/).

Here are some places to start:

### Themes

- To learn more about Gatsby themes specifically, we recommend checking out the [theme docs](https://www.gatsbyjs.com/docs/themes/).

### General

- **For most developers, we recommend starting with our [in-depth tutorial for creating a site with Gatsby](https://www.gatsbyjs.com/tutorial/).** It starts with zero assumptions about your level of ability and walks through every step of the process.

- **To dive straight into code samples, head [to our documentation](https://www.gatsbyjs.com/docs/).** In particular, check out the _Reference Guides_ and _Gatsby API_ sections in the sidebar.
