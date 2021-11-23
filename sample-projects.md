# Lab #3: Digital Exhibits (Sample Digital Exhibit/Archive Projects)

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.


# Table of Contents

- [Sample Digital Exhibit/Archive Projects](#sample-digital-exhibitarchive-projects)
  *  [Omeka](#omeka)
  *  [Static Sites](#static-sites)
     * [Wax](#wax)
     * [CollectionBuilder](#collectionbuilder)
  * [Sample Project Discussion/Reflection Questions](#sample-project-discussionreflection-questions)

# Sample Digital Exhibit/Archive Projects

Now, we're going to think about how we can use metadata to build digital archives/exhibits, thinking about...
- technical infrastructure
- metadata
- other information

## Omeka

The first digital archive platform or tool we're going to look at is Omeka.

Originally developed by George Mason University's Roy Rosensweig Center for History and New Media and initially released in 2008, "Omeka is a free, open-source content management system for online digital collections. As a web application, it allows users to publish and exhibit cultural heritage objects, and extend its functionality with themes and plugins" ([Wikipedia](https://en.wikipedia.org/wiki/Omeka)).

A few examples of Omeka in action:
- [Colored Conventions Project Digital Records](https://omeka.coloredconventions.org/)
- [Making Modern America: Discovering the Great Depression and New Deal](https://newdeal.oucreate.com/)
- [The Baseball Sheet Music Project](https://baseballsheetmusic.omeka.net/)

Most often, digital archive/exhibit projects built in Omeka use a metadata framework called Dublin Core, which can include the following fields:
- `Title`
- `Subject`
- `Description`
- `Creator`
- `Source`
- `Publisher`
- `Date`
- `Rights`
- `Format`
- `Language`
- `Type`
- `Identifier`
- `Coverage` (spatial or temporal)

For a more detailed explanation of these fields: Omeka Classic User Manual, "[Working With Dublin Core](https://omeka.org/classic/docs/Content/Working_with_Dublin_Core/)"

For more on Dublin Core: http://dublincore.org/about/

![omeka database screenshot](https://github.com/kwaldenphd/football-exhibits/blob/main/images/omeka_db.jpg?raw=true)

At the back-end, Omeka is driven by information that exists in tables that form a relational database.

Omeka's front-end development incorporates elements of PHP and jQuery to generate public-facing pages.

Omeka's full tech stack:
- Zend Framework
- getID3
- jQuery
- jQueryUI
- TinyMCE
- Silk Icons

For more on Omeka's technical infrastructure: https://github.com/omeka/Omeka

Omeka sandbox site for this lab:
- [Public site](http://kwaldenphd.com/omeka-classic-sandbox/)
- [Admin login](kwaldenphd.com/omeka-classic-sandbox/admin/)

## Static Sites

In the last few years, advocates of minimal computing principles have been thinking about other ways to create digital archives/exhibits that have less technical overhead than a content management system like Omeka.

Minimal computing is driven by "fundamental questions about choice and necessity," specifically:
- "What do we need?"
- "What don't we need?"
- "What do we want?"
- "What don't we want?"

(Jentery Sayers, "[Minimal Definitions](http://go-dh.github.io/mincomp/thoughts/2016/10/03/tldr/)" *Minimal Computing Working Group*, 3 October 2016)

Specifically, folks working in this area have been thinking about options that don't rely on relational databases or dynamically-generated web pages.

One of the things that has emerged from those conversations is static-site options for building digital archives/exhibits.

### Wax

Originally developed by digital scholarship librarians working at Columbia University and New York University, "Wax is an extensible workflow for producing scholarly exhibitions with minimal computing principles" ("[Wax](https://minicomp.github.io/wiki/wax/)", *Minicomp Wiki*).

From [the Wax documentation](https://minicomp.github.io/wiki/wax/)...
<em>
- The exhibition sites created by Wax are static.
  * This means they consist of flat HTML, CSS, and JavaScript files that don’t need to communicate in a complex way back to a server. This makes them cheaper, safer, and generally easier to maintain—as long as you’re willing to learn some new skills.

- The skills needed to create Wax sites are fundamental.
  * This means they are largely transferable for use in other digital projects. ‘Learning Wax’ does not mean learning how to use a platform. It involves learning the basics of web development, data management, and plain text editing while leveraging a few great open source libraries and frameworks along the way.

- Wax keeps the collection presentation separate from the collection data.
  * The Wax workflow starts with making standardized image files and metadata records and builds around them, handling canonical information, scholarly content, and site styling differently and deliberately. This makes it easier for you or others to reuse and reimagine your collection data in other contexts, or to preserve the collection when it comes time to sunset the exhibition.
</em>

Wax uses a combination of Ruby, Jekyll, and Rake.

![wax workflow diagram](https://github.com/kwaldenphd/football-exhibits/blob/main/images/wax_workflow.jpeg?raw=true)

Wax takes a spreadsheet with metadata and a collection of files (images, pdfs) and generates static pages for each item as well as a browsing and searching interface.

A few other resources folks might be interested in exploring at this point:
- [Sample Wax Site](https://minicomp.github.io/wax/)
- [Wax Documentation](https://minicomp.github.io/wiki/wax/)
- [Wax GitHub](https://github.com/minicomp/wax)

Let's take a look at a couple of sample sites built in Wax that use material from the University Archives.

### Bagby Negatives Wax Sandbox

Prof. Walden has prototyped a Wax site for the University Archive's [Bagby Glass Plate Negative Collection](http://archives.nd.edu/Bagby/index.htm).
- [Public site](https://kwaldenphd.github.io/wax-sandbox/)
- [GitHub](https://github.com/kwaldenphd/wax-sandbox)

There are two primary components that Wax uses to create this site: a spreadsheet with metadata and a folder with the image files

Metadata:
- [GitHub](https://github.com/kwaldenphd/wax-sandbox/blob/main/_data/photos.csv)
- [Google Drive](https://drive.google.com/drive/folders/1-3oFpWfjKFnact3tr7-zh7EdqGbHYerM?usp=sharing)

Image files:
- [GitHub](https://github.com/kwaldenphd/wax-sandbox/tree/main/_data/raw_images/bagby)
- [Google Drive](https://docs.google.com/spreadsheets/d/1a_Ss8WS3gwLgHYmoEtgFyj2g4ySOz9Htm_L6J1jN5Jw/edit?usp=sharing)

### Scholastic Football Review Wax Sandbox

Prof. Walden has also prototyped a Wax site for the [Scholastic Football Review issues from 1901-1931](http://archives.nd.edu/Football/).
- [Public site](https://kwaldenphd.github.io/wax-pdf-sandbox/)
- [GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox)

Again, there are two primary components driving the site: a spreadsheet with metadata and a folder with images created from the original PDFs.

Metadata:
- [GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox/blob/main/_data/scholastic.csv)
- [Google Drive](https://docs.google.com/spreadsheets/d/1vpT21C7pfCGqN26pLKiWrtLky-hCjGTsY-RhyfTNWpk/edit?usp=sharing)

Files:
- [GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox/tree/main/_data/raw_images/scholastic)
- [Google Drive](https://drive.google.com/drive/folders/1IJo7FGRMFd414xOU3U_omPxBUlbMlLGo?usp=sharing)

## CollectionBuilder

Another static site option for digital archives/exhibits is CollectionBuilder.

Developed by librarians at the University of Idaho, "CollectionBuilder is an open source tool for creating digital collection and exhibit websites that are driven by metadata and powered by modern static web technology" ([CollectionBuilder](https://collectionbuilder.github.io/))

From CollectionBuilder's ["About"](https://collectionbuilder.github.io/about.html) page:
<em>
- CollectionBuilder is a lightweight, flexible tool for creating digital collection websites that are driven by metadata and powered by modern static web technology. Using three primary components—a spreadsheet of metadata, a directory of assets, and a configuration file—CollectionBuilder gives information professionals and digital scholarship practitioners agency in building and customizing digital collection websites for free.

- CollectionBuilder is designed and maintained by librarians at the University of Idaho according to the Lib-STATIC approach, a methodology committed to leveraging static-web technologies and librarians’ specialized skills in metadata and classification to create engaging web publications.
</em>

CollectionBuilder uses a combination of Jekyll, GitHub, and Bootstrap for the core website components, and then integrates other open-source libraries (including DataTables, Leafletjs, lightGallery, TimelineJS) to generate other types of visualizations.

![collectionbuilder workflow diagram](https://github.com/kwaldenphd/football-exhibits/blob/main/images/collectionbuilder_workflow.jpg?raw=true)

Similar to Wax, CollectionBuilder takes a spreadsheet with metadata and a collection of files (images, pdfs) and generates static pages for each item as well as a browsing and searching interface.

A few other resources folks might be interested in exploring at this point:
- [Sample CollectionBuilder Site](https://collectionbuilder.github.io/collectionbuilder-gh/)
- [CollectionBuilder "About" page](https://collectionbuilder.github.io/about.html)
- [CollectionBuilder Documentation](https://collectionbuilder.github.io/cb-docs/)
- [CollectionBuilder GitHub](https://github.com/CollectionBuilder/collectionbuilder-gh)

Let's take a look at a couple of sample sites built in CollectionBuilder that use material from the University Archives.

### Bagby Negatives CollectionBuilder Sandbox

Prof. Walden has prototyped a CollectionBuilder site for the University Archive's [Bagby Glass Plate Negative Collection](http://archives.nd.edu/Bagby/index.htm).
- [Public site](https://kwaldenphd.github.io/collectionbuilder-sandbox/)
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-sandbox)

There are two primary components that Wax uses to create this site: a spreadsheet with metadata and a folder with the image files

Metadata:
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-sandbox/blob/main/_data/bagby_collectionbuilder.csv)
- [Google Drive](https://docs.google.com/spreadsheets/d/1idzbQRSBvW-_gpT-wl94PvE9UP22k3L_1ITwbObcCVU/edit?usp=sharing)

Image files:
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-sandbox/tree/main/objects)
- [Google Drive](https://drive.google.com/drive/folders/12XN0ap6FzBW2kpA3BcqgcgoPicP08vAh?usp=sharing)

### Scholastic Football Review CollectionBuilder Sandbox

Prof. Walden has also prototyped a CollectionBuilder site for the [Scholastic Football Review issues from 1901-1931](http://archives.nd.edu/Football/).
- [Public site](https://kwaldenphd.github.io/collectionbuilder-pdf-sandbox/)
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-pdf-sandbox)

In this case, CollectionBuilder is able to pull the PDF files from URLs that point to where these files exist on the ND Archives website, so the metadata is the primary component for the site and the files are pulled from the URLs.

Metadata:
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-pdf-sandbox/blob/main/_data/scholastic_collectionbuilder.csv)
- [Google Drive](https://docs.google.com/spreadsheets/d/1jOkBsxFs_76qwLqVTn7Eb1R1z8b0u4AJjLOZt0xRnl4/edit?usp=sharing)

## Sample project discussion/reflection questions

- Any questions or observations from this section of the lab
- Ideas that spark for how aspects of this work could be useful for telling a story about ND football
  * Or, aspects that might connect to some of the primary source materials we’ve been exploring
