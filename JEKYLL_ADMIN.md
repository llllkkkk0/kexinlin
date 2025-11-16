# Jekyll Admin Integration

This project now includes [Jekyll Admin](https://github.com/jekyll/jekyll-admin), a Jekyll plugin that provides a user-friendly admin interface for managing your Jekyll site.

## What is Jekyll Admin?

Jekyll Admin is a web-based administrative interface that makes it easier to manage your Jekyll site's content without directly editing files. It provides a graphical user interface for:

- Creating and editing blog posts
- Managing pages
- Uploading and organizing images and files
- Editing data files
- Configuring site settings
- Viewing and managing static files

## How to Access Jekyll Admin

1. **Start the Jekyll server:**
   ```bash
   bundle exec jekyll serve
   ```

2. **Access the admin interface:**
   Open your browser and navigate to:
   ```
   http://localhost:4000/admin
   ```

3. **Manage your content:**
   Use the intuitive interface to create, edit, and manage your site's content.

## Features

- **Posts Editor**: Create and edit blog posts with a rich text editor
- **Pages Manager**: Manage your site's pages
- **Collections**: Work with Jekyll collections
- **Data Files**: Edit YAML, JSON, and CSV data files
- **Static Files**: Upload and manage images, PDFs, and other assets
- **Configuration**: View and edit your `_config.yml` file
- **Metadata Editor**: Easily manage front matter for posts and pages

## Production Deployment

**Important:** Jekyll Admin should only be used in development environments. For security reasons, it's automatically disabled when `JEKYLL_ENV=production` is set.

When deploying to GitHub Pages or other production environments, Jekyll Admin will not be included in the build.

## Documentation

For more information about Jekyll Admin, visit:
- [Official Documentation](https://github.com/jekyll/jekyll-admin)
- [Jekyll Admin Demo](http://jekyll.github.io/jekyll-admin/)

## Troubleshooting

If you encounter issues accessing the admin interface:

1. Make sure the Jekyll server is running
2. Verify that you're accessing `http://localhost:4000/admin` (not just `/admin`)
3. Check that `jekyll-admin` is listed in your Gemfile
4. Run `bundle install` to ensure all dependencies are installed
5. Clear your browser cache and try again

## Changes Made

The following changes were made to integrate Jekyll Admin:

1. Added `jekyll-admin` gem to the `Gemfile` in the `:jekyll_plugins` group
2. Ran `bundle install` to install Jekyll Admin and its dependencies
3. The plugin is automatically loaded by Jekyll when the server starts

No additional configuration is required in `_config.yml` - Jekyll Admin works out of the box!
