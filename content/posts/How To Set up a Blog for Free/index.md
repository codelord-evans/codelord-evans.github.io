---
title: "How To Setup a Blog for Free"
date: 2023-08-23T13:58:34+03:00
draft: false
---

>  "Free things often come at the highest price."

In the digital age, starting a blog has become easier than ever before. Thanks to the availability of powerful and free tools, you can create and host your own blog without breaking the bank. In this step-by-step guide, we will explore how to set up a blog for free using Hugo, a popular static site generator, and GitHub Pages for hosting. By the end of this tutorial, you'll have a fully functional blog that you can customize to your heart's content.

## What You'll Need

Before we dive into the setup process, here's a list of prerequisites:

1. **GitHub Account:** If you don't have one already, sign up for a GitHub account at [github.com](https://github.com/).

2. **Hugo:** Install Hugo by following the instructions for your specific operating system on the [official Hugo website](https://gohugo.io/getting-started/installing/).

3. **Basic Text Editor:** You'll need a basic text editor to create and edit your blog posts. You can use anything from Notepad to more advanced text editors like Visual Studio Code or Sublime Text.

4. **Command Line (Optional):** Some familiarity with the command line will be helpful, but it's not mandatory. You can perform most tasks through the Hugo interface.

## Step 1: Create a New GitHub Repository

1. Log in to your GitHub account.

2. Click the "New" button to create a new repository.

3. Choose a name for your repository. It's a good practice to name it something related to your blog, e.g., "my-awesome-blog."

4. Make sure the repository is public, as GitHub Pages hosting requires public repositories.

5. Optionally, you can add a README file, which is useful for documenting your project.

6. Click the "Create repository" button.

## Step 2: Clone Your GitHub Repository

Now that you have created your repository, you need to clone it to your local machine.

1. Click the green "Code" button on your repository's page.

2. Copy the repository URL (it should look like `https://github.com/your-username/my-awesome-blog.git`).

3. Open your terminal/command prompt and navigate to the directory where you want to store your blog project.

4. Run the following command, replacing `<repository-url>` with the URL you copied in step 2:

   ```
   git clone <repository-url>
   ```

## Step 3: Initialize Hugo in Your Repository

1. Open your terminal/command prompt and navigate to the directory where you cloned your GitHub repository in step 2.

2. Run the following command to initialize Hugo in your repository:

   ```
   hugo new site .
   ```

3. Hugo will create the necessary folder structure and configuration files for your blog.

## Step 4: Choose a Hugo Theme

Hugo offers a wide variety of themes to choose from. You can find Hugo themes on the [Hugo Themes website](https://themes.gohugo.io/). Here's how to add a theme to your blog:

1. Visit the Hugo Themes website and find a theme that you like.

2. Once you've chosen a theme, go to its GitHub repository.

3. Copy the repository URL.

4. Inside your blog's project directory, run the following command to add the theme as a submodule, replacing `<theme-url>` with the URL you copied:

   ```
   git submodule add <theme-url> themes/<theme-name>
   ```

5. Open the `config.toml` file in the root directory of your blog and set the `theme` parameter to the name of your chosen theme.

## Step 5: Create Your First Blog Post

Now that you have your blog set up and a theme in place, let's create your first blog post:

1. Run the following command to create a new blog post:

   ```
   hugo new posts/my-first-post.md
   ```

2. This will create a new Markdown file in the `content/posts/` directory with a template for your blog post.

3. Open the Markdown file in your text editor and start writing your blog post. You can use Markdown syntax to format your content.

## Step 6: Customize Your Blog

Hugo provides extensive customization options. You can modify the appearance and functionality of your blog by editing the theme's templates, CSS files, and configuration files. Refer to the theme's documentation for specific instructions on customization.

## Step 7: Build Your Blog

To generate the static files for your blog, run the following command in your project's root directory:

```
hugo
```

This will create a `public` directory with all the HTML, CSS, and other assets needed for your blog.

## Step 8: Push Your Changes to GitHub

Now it's time to push your blog to GitHub:

1. Add all the changes to your Git repository:

   ```
   git add .
   ```

2. Commit your changes:

   ```
   git commit -m "Initial commit"
   ```

3. Push your changes to GitHub:

   ```
   git push origin main
   ```

## Step 9: Configure GitHub Pages

1. Go to your GitHub repository's Settings.

2. Scroll down to the "GitHub Pages" section.

3. Under "Source," select the branch where your Hugo-generated files are stored. It's typically the `main` branch.

4. Set the folder to `/docs` or `/public`, depending on your Hugo version.

5. Click the "Save" button.

## Step 10: Access Your Blog

Once GitHub Pages has deployed your site (which may take a few minutes), you can access your blog at `https://your-username.github.io/my-awesome-blog` (replace `your-username` with your GitHub username and `my-awesome-blog` with your repository name).

Congratulations! You've successfully set up a free blog using Hugo and GitHub Pages for hosting. You can continue to write and publish blog posts by following the same process outlined in step 5. Additionally, you can explore Hugo's documentation and your chosen theme's documentation to further customize your blog and make it truly your own. Happy blogging/ Coding!