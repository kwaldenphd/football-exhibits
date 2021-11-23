## Static Sites

Note on scope: You're not being asked to develop a full-scale functioning project here. Folks working on this task should expect to spend 1-2 hours working on the static site you're buliding.

At this point, the person who is the GitHub wrangler or point person for your group should have made a copy (fork) of a repository for the platform you're using and have gone through the necessary software installs.

### Technical Infrastructure

At least one person in your group should set up a GitHub account and fork one of the sample repositories for the lab’s static sites.

- [Wax](https://github.com/kwaldenphd/football-exhibits#wax)
  * Bagby Glass Plates ([public site](https://kwaldenphd.github.io/wax-sandbox/), [GitHub](https://github.com/kwaldenphd/wax-sandbox))
  * Scholastic Football Review ([public site](https://kwaldenphd.github.io/wax-pdf-sandbox/), [GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox))

- [CollectionBuilder](https://github.com/kwaldenphd/football-exhibits#collectionbuilder)
  * Bagby Glass Plates ([public site](https://kwaldenphd.github.io/collectionbuilder-sandbox/), [GitHub](https://github.com/kwaldenphd/collectionbuilder-sandbox))
  * Scholastic Football Review ([public site](https://kwaldenphd.github.io/collectionbuilder-pdf-sandbox/), [GitHub](https://github.com/kwaldenphd/collectionbuilder-pdf-sandbox))

The same person/people will also need to go through the software install steps for the static site platform you’re choosing. 
- [Wax](https://minicomp.github.io/wiki/wax/setting-up-your-system/)
- [CollectionBuilder](https://collectionbuilder.github.io/cb-docs/docs/software/)

Lab #3 Software Installs:
- Git (specifically Git Bash and GitHub Desktop)
- Ruby
- Jekyll
- ImageMagick
- Ghostscript
- For Wax: Libvips

- Documentation
  * [Wax Install Guide](https://minicomp.github.io/wiki/wax/setting-up-your-system/install-manually/)
  * [CollectionBuilder Install Guide](https://collectionbuilder.github.io/cb-docs/docs/software/)

### Wax

Step 1: Prepare collection data ([metadata](https://minicomp.github.io/wiki/wax/preparing-your-collection-data/metadata/) and [directory of files](https://minicomp.github.io/wiki/wax/preparing-your-collection-data/image-data/))
- [Documentation](https://minicomp.github.io/wiki/wax/preparing-your-collection-data/)
- [Google Drive folder with files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Google Drive folder with starter metadata for ND Archive collections](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)
- [Metadata Templates](https://drive.google.com/drive/folders/1NuVx0qiOBahf0neMnT9RYF_VlwkgiiVv?usp=sharing)
- Sample Metadata
  * Image files ([GitHub](https://github.com/kwaldenphd/wax-sandbox/blob/main/_data/photos.csv), [Google Drive](https://drive.google.com/drive/folders/1-3oFpWfjKFnact3tr7-zh7EdqGbHYerM?usp=sharing))
  * PDF files ([GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox/blob/main/_data/scholastic.csv), [Google Drive](https://docs.google.com/spreadsheets/d/1vpT21C7pfCGqN26pLKiWrtLky-hCjGTsY-RhyfTNWpk/edit?usp=sharing))

Step 2: Modify the demo template
- [Clone the repository from GitHub.com to GitHub Desktop](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop)
- [Swap in your collection data](https://minicomp.github.io/wiki/wax/setting-up-your-site/adding-your-collection-data/)
- [Update your configuration](https://minicomp.github.io/wiki/wax/setting-up-your-site/updating-your-configuration/)
  * Specifically, you'll need to modify the following files:
    * `_config.yml`
    * `index.md` (swap out your collection name, the banner image, and home page text)
    * `collection.md` (swap out your collection name in the `{% include collection_gallery.html collection='bagby' facet_by='_date' %}` line)
    * Optional: If you want a custom layout for each item page, you'll also want to modify the `bagby_item.html` file in the `_layouts` folder. [Link to more documentation on layouts](https://minicomp.github.io/wiki/wax/using-theme-layouts/).

Step 3: [Build the site](https://minicomp.github.io/wiki/wax/running-the-tasks/)
- You'll need to run the following three rake tasks within Git BASH before pushing those updates from GitHub Desktop to the online GitHub repository
  * [Create image derivatives and update metadata](https://minicomp.github.io/wiki/wax/running-the-tasks/derivatives/) (`wax:derivatives`)
  * [Create pages](https://minicomp.github.io/wiki/wax/running-the-tasks/pages/) (`wax:pages`)
  * [Create search index](https://minicomp.github.io/wiki/wax/running-the-tasks/search/) (`wax:search`)

Step 4: Configure GitHub pages and publish the site
- [Set up GitHub repository for GitHub Pages](https://minicomp.github.io/wiki/wax/serving/#with-github-pages)
- [Push changes from GitHub Desktop to GitHub repository](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/pushing-changes-to-github)

Step 5: Visit your new site (and continue to refine as needed)
- URL structure: https://`your github username`.github.io/`your repository name`
- Sample: https://kwaldenphd.github.io/wax-sandbox/

### Collection Builder

Step 1: Prepare collection data ([metadata](https://collectionbuilder.github.io/cb-docs/docs/metadata/gh_metadata/) and if needed [directory of files](https://collectionbuilder.github.io/cb-docs/docs/objects/gh-objects/))
- [Documentation](https://collectionbuilder.github.io/cb-docs/docs/metadata/gh_metadata/)
- [Google Drive folder with files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Google Drive folder with starter metadata for ND Archive collections](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)
- [Metadata Templates](https://drive.google.com/drive/folders/1NuVx0qiOBahf0neMnT9RYF_VlwkgiiVv?usp=sharing)
- Sample Metadata
  * From files ([GitHub](https://github.com/kwaldenphd/collectionbuilder-sandbox/blob/main/_data/bagby_collectionbuilder.csv), [Google Drive](https://docs.google.com/spreadsheets/d/1idzbQRSBvW-_gpT-wl94PvE9UP22k3L_1ITwbObcCVU/edit?usp=sharing))
  * From URLs ([GitHub](https://github.com/kwaldenphd/collectionbuilder-pdf-sandbox/blob/main/_data/scholastic_collectionbuilder.csv), [Google Drive](https://docs.google.com/spreadsheets/d/1jOkBsxFs_76qwLqVTn7Eb1R1z8b0u4AJjLOZt0xRnl4/edit?usp=sharing))

Step 2: Modify the demo template
- Clone the repository from GitHub.com to GitHub Desktop ([GitHub documentation](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop), [CollectionBuilder documentation](https://collectionbuilder.github.io/cb-docs/docs/repository/clone/))
- [Open the repository](https://collectionbuilder.github.io/cb-docs/docs/repository/open/)
- [Swap in your collection data](https://collectionbuilder.github.io/cb-docs/docs/objects/gh-objects/)
- [Update your configuration](https://collectionbuilder.github.io/cb-docs/docs/config/)
- [Update pages](https://collectionbuilder.github.io/cb-docs/docs/theme/)
  * Specifically, you'll need to modify the following files:
    * [`_config.yml`](https://collectionbuilder.github.io/cb-docs/docs/config/)
    * To update the homepage (`home-infographic.html`, in `_layouts` folder): https://collectionbuilder.github.io/cb-docs/docs/theme/home, https://collectionbuilder.github.io/cb-docs/docs/pages/home
    * To update the "About" page (`about.md` in `pages` folder): https://collectionbuilder.github.io/cb-docs/docs/pages/interpretive/#about-page
    * To update the `theme.yml` file (in the `_data` folder): https://collectionbuilder.github.io/cb-docs/docs/theme/
      * You may also want to take a look at and potentially modify the `csv` files in the `_data` folder (`config-browse`, `config-map`, `config-metadata`, `config-nav`, `config-search`, `config-table`, `config-theme-colors`)
      * https://collectionbuilder.github.io/cb-docs/docs/customization/
      * https://collectionbuilder.github.io/cb-docs/docs/pages/

Step 3: Configure GitHub pages and publish the site
- [Set up GitHub repository for GitHub Pages](https://collectionbuilder.github.io/cb-docs/docs/deploy/gh-pages/)
- [Push changes from GitHub Desktop to GitHub repository](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/making-changes-in-a-branch/pushing-changes-to-github)

Step 5: Visit your new site (and continue to refine as needed)
- URL structure: https://`your github username`.github.io/`your repository name`
- Sample: https://kwaldenphd.github.io/collectionbuilder-sandbox/
