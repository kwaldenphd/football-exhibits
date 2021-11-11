# Lab #3: Digital Exhibits

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
This tutorial is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

# Overview

This lab will involve working with digital archive and exhibit platforms and tools to think about avenues for presenting or sharing historical work. Specifically, it focuses on workflows for building out item-level metadata needed to generate a robust digital archive/exhibit and prototyping options for sharing or presenting that work using digital exhibits and interactive digital storytelling tools. 

This lab provides a few different types of open-ended opportunities for thinking about how to share/communicate/present information related to primary source materials, in a smaller-scale, lower-stakes setting than the final project. I encourage folks to approach this lab as a pilot or “proof of concept” for work they might want to continue or develop further in the final project.

# Table of Contents

- [How To Work Through This Lab](#how-to-work-through-this-lab)
  * [Lab Timeline](#lab-timeline)
  * [Lab Notebook Components](#lab-notebook-components)
- [Background](#background)
- [Metadata](#metadata)
  * [What is Metadata?](#what-is-metadata)
  * [Metadata in Action](#metadata-in-action)
  * [Metadata Reflection Questions](#metadata-reflection-questions)
- [Sample Digital Exhibit/Archive Projects](#sample-digital-exhibitarchive-projects)
  *  [Omeka](#omeka)
  *  [Static Sites](#static-sites)
     * [Wax](#wax)
     * [CollectionBuilder](#collectionbuilder)
  * [Sample Project Discussion/Reflection Questions](#sample-project-discussionreflection-questions)
* [Immersive or Interactive Digital Stories](#immersive-or-interactive-digital-stories)
  * [TimelineJS](#timelinejs)
  * [StoryMapJS](#storymapjs)
  * [ArcGIS StoryMaps](#arcgis-storymaps) 
  * [Open-Source Alternatives](#open-source-alternatives)
  * [And so much more!](#and-so-much-more)
- [Next Steps](#next-steps)
  * [Static Site](#static-site)
  * [Omeka Collection or Exhibit](#omeka-collection-or-exhibit)
  * [Immersive or Interactive Digital Story](#immersive-or-interactive-digital-story)  

# How to Work Through This Lab

[Link to Google Drive workspace for this lab](https://drive.google.com/drive/folders/13uxuOwLOO6taBSmj-8OvDnWf7EcKQZu3?usp=sharing)

This lab is organized into three main sections:
- What's possible under the umbrella of digital archives, digital exhibits, and immersive/interactive digital storytelling
- What's involved in building these kinds of projects or components
- What might be possible with these tools/approaches and primary sources or archival material related to ND football

So the lab starts by looking at existing digital projects that incorporate these tools/methods, to think about what might be possible related to the work of this class.

Then, folks will have a chance to work behind-the-scenes with building these types of projects.

In that behind the scenes work, we'll be thinking about...
- The technical infrastructure needed to publish these projects
- The metadata that drives these projects
- What types of contextual or narrative information is also part of these projects

Lastly, folks will have a chance to take up these methods to source material of your choosing that relates to ND football.

As we think about how you could take up or extend these methods, we'll be doing that with an eye toward the final project.

## Lab Timeline

We'll spend two Thursday class periods working on this lab: 10/28 and 11/4.

Ideally we're finishing up this lab during Week #12 (week of 11/8) so we can turn and start to focus on the final project. 

## Lab Notebook Components

- Reflections/observations from the Background section of the lab
- Reflections/observations from the Metadata section of the lab
- Reflections/observations from your work exploring tools and sample projects
- Your group's work building out digital exhibit/archive and immersive/interactive digital story
  * Any data files you worked with
  * Public-facing things you created (GitHub Pages site, Omeka collection/exhibit, StoryMap, timeline, etc)
- Individual reflection
  * At least 200 words (or 2-3 minutes audio/video), addressing the following questions:
    * What you learned about metadata through this lab
    * What you learned about digital exhibits/archives through this lab
    * What you learned about immersive/interactive digital storytelling through this lab
    * How you're thinking about these tools/approaches as they relate to ND football history and primary sources differently after this lab
    * Where you would go next with these tools/methods (other research questions/topics you're interested in exploring, other data sources or types of data you would want to be able to work with, etc)
    * Other comments/questions/observations

If you're working in Google Drive, you can just submit a link to Google Drive.

Notebooks can be individual or collaborative.

# Background

Explore...
- [One of the Colored Conventions Projects exhibits](https://coloredconventions.org/exhibits/) (many to choose from!)
- [One of the place-based walking tour projects](https://curatescape.org/projects/)
- [One of the interactive digital stories built using ArcGIS StoryMaps](https://www.esri.com/en-us/arcgis/products/arcgis-storymaps/albums/digital-humanities)

As you explore, consider…
- What types of sources it uses, and how it uses those sources (interactive maps/visualizations, text, immersive media, etc)
- Choices the authors/creators made around design and presentation, and how that shapes the user experience 
  * To put that another way, what are some of your takeaways from engaging with the project? What aspects of the project stand out to you (and how/why)?
- Ideas that spark for how aspects of what this project is doing could be useful for telling a story about ND football
  * Or, aspects of the project design/composition that might connect to some of the primary source materials we’ve been exploring 

# Metadata

## What is Metadata?

Metadata is often defined or described as "data that provides information about other data" ([Merriam Webster](https://www.merriam-webster.com/dictionary/metadata)).

Within the world of digital information systems, "metadata, the information we create, store, and share to describe things, allows us to interact with these things to obtain the knowledge we need" (Jenn Riley, "[Understanding Metadata: What is Metadata, and What is it For?: A Primer](http://www.niso.org/publications/understanding-metadata-2017)" *National Information Standards Organization*, 2017).

To think about this another way, "In essence, metadata is the extra baggage associated with any resource that enables a real or potential user to find that resource; to decide whether or not it is of value to them; to discover where, when and by whom it was created, as well as for what purpose; to know what tools will be needed to manipulate the resource; to determine whether or not they will actually be allowed access to the resource itself and how much this will cost them. Metadata is, in short, a means by which largely meaningless data may be transformed into information, interpretable and reusable by those other than the creator of the data resource" (Paul Miller, "Metadata: What it Means for Memory Institutions" in *Metadata Applications and Management*, 2004).

From the "[Metadata & Discovery](https://pitt.libguides.com/metadatadiscovery/)" University of Pittsburgh Library Guide authored by Mike Bolam:
<em>
- Metadata aids in managing, publicizing, and preserving the content you have produced. It enhances the usefulness of your data or information by providing context—the who, what, when, where, why, and how that helps to discover, identify, interpret, and interact with content.

- Metadata allows users to:
 * Find or identify a resource
 * Know who created the resource or contributed to the creation of the resource
 * Understand how the resource was created and manipulated
 * Know when the resource was created
 * Determine tools needed to view, manipulate, and use the resource
 * Understand rights and use conditions surrounding the resource
 * Connect to related information objects
</em>

## Metadata in Action

Let's look at a couple examples of metadata in action.

### ND Library Catalog Record

First, open [the ND Library catalog record for Sperber's *Shake Down the Thunder*](https://onesearch.library.nd.edu/permalink/f/1phik6l/ndu_aleph001373767) in a web browser.

Think about what types of information show up in the record for Sperber's book. 
- Information about the book itself
- Information about its location, status, or condition
- Etc.

Since the 1960s, machine readable cataloging (or MARC) records have been the back-bone for library interface and discovery systems.

![physical card from card catalog](https://github.com/kwaldenphd/football-exhibits/blob/main/images/card_catalog.jpg?raw=true)

MARC records developed as a way of taking the information represented in a card catalog and moving it into a digital or computer-aided discovery environment.

![MARC punch chard from University of Kansas Libraries](https://github.com/kwaldenphd/football-exhibits/blob/main/images/marc_punch.png?raw=true)

While MARC records started as physical punch cards, in the last 30 years, MARC records that functioned as databases continue to evolve and transform via the internet.

```
Leader 00000cam a2200445Ia 4500
005    20200930030738.0
008    960111s1995    nyuaf    b    001 0 eng d
010    ##$z93027979
019    ##$a614890556
020    ##$z0805018743
020    ##$z0805042431
035    9#$aAGG4526
035    ##$a(OCoLC)34017897
040    ##$aIND$beng$cIND$dBTCTA$dYDXCP$dOCLCQ$dOCLCF$dOCLCQ$dADU$dBDX$dOCLCO$dIOL$dYCP$dOCLCQ$dIND
043    ##$an-us-in
049    ##$aINDU
050    #4$aGV958.N6$bS64 1995
082    04$a796.332/63/0977289$220
100    1#$aSperber, Murray.
245    10$aShake down the thunder :$bthe creation of Notre Dame football /$cMurray Sperber.
250    ##$a1st Owl book ed.
260    ##$aNew York :$bHenry Holt and Co.,$c1995.
300    ##$axxii, 634 pages, 8 unnumbered pages of plates :$billustrations ;$c23 cm
336    ##$atext$btxt$2rdacontent
337    ##$aunmediated$bn$2rdamedia
338    ##$avolume$bnc$2rdacarrier
504    ##$aIncludes bibliographical references (pages 503-617) and index.
505    0#$a1. "What though the odds be great or small": 1789-1918. L'Universite de Notre Dame du Lac and the nineteenth century -- The origins of Notre Dame's athletic culture -- Catholic versus American higher education -- The origin of the "Notre Dame victory march" -- Notre Dame sports: 1900-1912 -- Jesse Harper: 1913 and the first Army game; 1914 and the finances of college football; 1915-1917 and the job of athletic director -- Jesse Harper's assistant: Knute Rockne. 2. Shaking down the thunder: 1918-1931. Catholic versus American higher education in the 1920s -- The growth of the athetic culture -- The origin of the "Fighting Irish" nickname -- Rockne at ground zero: 1918-1919 -- Rockne's rocket, first version: 1920 -- George Gipp's five seasons at Notre Dame -- The rocket crashes, Rockne's miraculous escape: 1921 -- Building a better rocket: 1922 -- On the launch pad: 1923 -- Notre Dame versus Klandiana: 1924 -- Blast off: 1924.
505    0#$aThe four horsemen, Grantland Rice versus reality -- Rockne threatens to jump ship: 1925 -- Anti-aircraft fire from the Big Ten: 1926 -- Knute K. Rockne Inc. -- Anti-aircraft fire from the college sports reformers: 1927 -- Al Smith and "win one for the Gipper": 1928 -- Rockne attacks the college sports reformers: 1929 -- Rockne's last and greatest rocket: 1930 -- The death of reform and Rockne. 3. "Rally sons of Notre Dame": 1932-1941. In the Depression: 1931-1941 -- After Rockne in 1931 -- The demand for perfection: 1932 -- The removal of a vice president and the first firing of a Note Dame head coach: 1933 -- O'Hara and Layden assume power: 1934-1936 -- ... in power: 1937-1939 -- Beginning and filming Knute Rockne, all American: 1939-1940 -- The end of the Rockne era: 1940 -- The end of the creation of Notre Dame football: 1941.
590    ##$aHesburgh Collection has author's signed presentation copy with inscription.
610    20$aUniversity of Notre Dame$xFootball$xHistory.
610    20$aNotre Dame Fighting Irish (Football team)$xHistory.
655    #7$aHistory.$2fast$0(OCoLC)fst01411628
852    00$aInNd$bSPEC$cHESB$hGV 958 .N6 S64 1995
938    ##$aBrodart$bBROD$n48220140$c$15.95
938    ##$aBaker and Taylor$bBTCP$nbl 99767160
938    ##$aYBP Library Services$bYANK$n675865
994    ##$aC0$bIND
AVA    ##$aNDU50$bSPEC$cHesburgh Collection$dGV 958 .N6 S64 1995$echeck_holdings$tCheck Holdings$jHESB$k0
FMT    BK
LDR         cam a2200445Ia 4500
TYP    ##$aBook
XYZ    ##$aNotre Dame (Ind.).$bUniversity of Notre Dame
XYZ    ##$aNotre Dame University
XYZ    ##$aNotre Dame, Ind.$bUniversity
XYZ    ##$aSouth Bend (Ind.).$bUniversity of Notre Dame
XYZ    ##$aSouth Bend (Ind.).$bNotre Dame University
XYZ    ##$aUniversity of Notre Dame du Lac
XYZ    ##$aNotr-Damskiĭ universitet
XYZ    ##$aIrish (Football team)
XYZ    ##$aUniversity of Notre Dame.$bFighting Irish (Football team)
XYZ    ##$aFighting Irish (Football team)
```

An example of the [digital MARC record for Sperber's book](https://onesearch.library.nd.edu/primo-explore/sourceRecord?vid=NDU&docId=ndu_aleph001373767), that drive the ND Library catalog record.

### Marble

Another example of metadata in action is [Marble (Museums, Archives, Rare Books, and Libraries Exploration), ND's new digital collections platform](https://marble.nd.edu/) that brings together materials from the Snite Museum of Art, the University's Rare Books and Special Collections, and the University Archive.

From [the ND press release about Marble's launch](https://news.nd.edu/news/notre-dame-launches-platform-for-online-access-to-library-museum-holdings/):
<em>
- University libraries, archives and museums nationwide have been digitizing collections for well over a decade and have long sought collaborative solutions that would enable their respective holdings to be easily discovered online and used for teaching and research. However, there have been many obstacles preventing efficient and expansive research across collections, including disparate technical systems, discipline-specific practices and descriptive metadata norms.

- Faculty, students and the general public can browse Marble and download select digitized materials from the Snite Museum of Art, Rare Books & Special Collections and the University Archives in a single platform — including books, manuscripts, sculptures, paintings, photographs, ephemera and more. Each item displays one or more images with descriptive information and linked metadata to view related or similar items.

- The Marble software...uses a harvest model to draw descriptive information from key source systems and features a shared administrative back-end to augment harvested data. This solution is possible due to a shared understanding of different descriptive terms.

</em>

To learn more about Marble's origins and technical infrastructure:
- Tara O'Leary and Jenna Mrozinske, "[Notre Dame launches platform for online access to library, museum holdings](https://news.nd.edu/news/notre-dame-launches-platform-for-online-access-to-library-museum-holdings/)" *Notre Dame News* (21 July 2021)
- [OSF repository](https://osf.io/cusmx/)
- [GitHub](https://github.com/ndlib/marble-website-starter)
- [Mikala Narlock, Digital Collections Strategy Librarian](https://directory.library.nd.edu/directory/employees/mnarlock)

### University Archives

Now, by way of comparison, let's head to the "[Digital Collections](http://archives.nd.edu/digital/)" page for the University Archives.

Compare your experience navigating this interface and accessing materials to using the University Library catalog or Marble system.

Those vastly different user experiences or ways of engaging/access materials are driven by two key components: technical infrastructure and metadata.

## Metadata Reflection Questions

- Any questions or observations from this section of the lab
- Ideas that spark for how aspects of this work could be useful for telling a story about ND football
  * Or, aspects that might connect to some of the primary source materials we’ve been exploring 

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

# Immersive or Interactive Digital Stories

The last type of digital exhibit we're going to look at and think about for this lab are immersive or interactive digital stories.

Digital storytelling is a VERY BROAD term that can include everything from podcasts to video essays.

In this lab, we're going to focus on immersive or interactive digital stories that are either driven by metadata and/or operate as a media-rich long-form narrative.

Earlier in this lab, you/your group looked at some of the  [interactive digital stories built using ArcGIS StoryMaps](https://www.esri.com/en-us/arcgis/products/arcgis-storymaps/albums/digital-humanities).
- NOTE: You could also use open-source tools to generate some of the features/functionality you're seeing in StoryMaps.
  * [An example built using JavaScript](https://bostonopioid.github.io/discarded-needle/index.html)
  * [Juncture platform that stitches together JavaScript and Jekyll and integrates with GitHub Pages](https://juncture-digital.org/)
- ANOTHER NOTE: An alternate platform that is well-suited to media-rich immersive long-form narratives (but does not support interactive mapping) is Adobe Spark
  * [Example](https://spark.adobe.com/page/OVvbwUF0Qo1Cs/)
  * [Tutorial](https://remix.nd.edu/photo-essay.html)

A few other types of work that might fall under this umbrella...

**Timelines**

- Platform: [TimelineJS](http://timeline.knightlab.com/) (Northwestern's Knight Lab)
- Example: [Notre Dame 1968 Timeline](http://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1MPga-KBhpiRiEK-caa_oPJawa8z129D1EnFzppi6YjU&font=Default&lang=en&initial_zoom=2&height=850&fbclid=IwAR1RDYYtV7cntvxMtXibUxXJjXEulZys-skG0qAL06nm-ksHIWqO0MxkJns)
- Tutorial: https://remix.nd.edu/interactive-timeline.html

**Map**

Platform: [StoryMapJS](http://storymap.knightlab.com/) (Northwestern's Knight Lab)

Examples:
- [Fists of Freedom: Reactions to John Carlos and Tommie Smith's 1968 Protest, Dr. Louis Moore](https://uploads.knightlab.com/storymapjs/3107230e5eafea9f5e74496d4a1a0f40/black-fists/index.html)
- [Black Athletes, Housing, and Racial Discrimination, Dr. Louis Moore](https://uploads.knightlab.com/storymapjs/3107230e5eafea9f5e74496d4a1a0f40/black-athletes-and-housing/index.html)

Tutorial: https://lindseywieck.org/fall_2016_sf/storymapjstutorial.html

Platform: [CurateScape, built on Omeka](https://curatescape.org)

Examples:
- [Prof. Walden's sandbox site](http://kwaldenphd.com/curatescape-sandbox/)
- [College of Charleston](https://curatescape.org/projects/discovering-our-past-college-of-charleston-histories/)
- [Muhlenberg College](https://curatescape.org/projects/muhlenberg-pathways-to-present/)
- [Curatescape Project Directory](https://curatescape.org/projects/)

Tutorial: 
- [CurateScape documentation](https://curatescape.org/docs/content-creation-guide/)
- [University of Oregon Library Guide](https://researchguides.uoregon.edu/c.php?g=900917&p=6482491)

**Interactive Data Visualization**

Platform (with example): [StorylineJS](http://storyline.knightlab.com/) (Northwestern's Knight Lab)

NOTE: You could also generate annotated interactive visualizations programmatically using Plotly in Python or RStudio.
- [Python](https://plotly.com/python/text-and-annotations/)
- [RStudio](https://plotly.com/ggplot2/text-and-annotations/)

**360 photo/video**

There's also a whole world of 360 photo/video and virtual reality adjacent work that might fall under the digital storytelling umbrella.

A few user-friendly tools that support 360 photo/video:
- [SceneVR](https://scene.knightlab.com/) (Northwestern's Knight Lab)
- [Story Spheres](https://storyspheres.com/)
- [Google Cardboard Camera app](https://blog.google/products/google-ar-vr/cardboard-camera-ios/)

There's also a whole other world of more advanced tech applications in the area of [VR/MR/AR/XR](https://medium.com/@effinmickey/vr-ar-mr-xr-and-360-everything-youve-always-wanted-to-know-ae33e4515493) and [photogrammetry](https://rd.nytimes.com/projects/an-end-to-end-guide-to-photogrammetry-with-mobile-devices).

## Immersive/Interactive Digital Stories Reflection Questions

- Any questions or observations from this section of the lab
- Ideas that spark for how aspects of this work could be useful for telling a story about ND football
  * Or, aspects that might connect to some of the primary source materials we’ve been exploring 

# Next Steps

Now it's your turn to work in your group to begin exploring what might be possible with these tools/approaches and primary sources (or archival material) related to ND football.

Each group is asked to build out three different types of digital exhibits as part of this lab.

**#1: Spin up a working instance of Wax or CollectionBuilder OR substantively modify/expand Prof. Walden's sandbox sites.**

For #1, some of the things that you'll need to build out along the way will include...
- Site text
- Metadata
- Pages/configuration

**#2: Develop a Omeka Collection based on ND Archive materials**

For #2, some of the things that you'll need to build out along the way will include...
- Metadata
  * Potentially also exhibit curation/configuration

**#3: Build a small-scale immersive/interactive digital story**

Options include:
- Adobe Spark
- ArcGIS StoryMaps
- Timeline JS
- Storymap JS
- Storyline JS
- Curatescape (built on Omeka)
- Something open-source/homegrown
- If you want to dabble in 360/VR/AR/MR
  * StorySphere
  * SceneVR
  * Etc

For #3, some of the things that you'll need to build out along the way might include...
- Object inventory
- Design/visual content
- Text
- Interactive map(s)
- Metadata

## Collaborating Well

Collaboration is also your friend here- you don't have to come up with all the ideas or do all the work on your own. For example, CDT/CSE folks can focus on building out the technical infrastructure for the static sites. Data Science folks (or folks comfortable working with structured data) can focus on building on the metadata. Folks who want to think about front-end presentation or user experience could focus on task #3 and provide input on things like exhibit text, page layout, item tags, etc. for #1 and #2.

In short, leverage the group's strengths. And divide/conquer.

Folks are welcome to meet with me (individually or as a group) to ask questions and think about next steps for how to approach this lab.

## Where to Start: Selecting Materials

The first step is figuring out what materials you want to work with for tasks #1 and #2.

Each collection has Google Drive links for the bulk downloaded files and starter metadata.

NOTE: If you are planning on working using the Scholastic student magazine or Observer student newspaper to create a static site in Wax, you will need to select a subset of years to avoid hitting GitHub repository limits (and avoid crashing the Rake tasks)
- CollectionBuilder can pull from URLs so you won't have the same issue

### Alumnus

From the [University Archives](http://archives.nd.edu/digital/):
- "The Alumnus, published by the Alumni Association from January of 1923 until December of 1971, provided news and feature articles of interest to Notre Dame graduates. Notre Dame Magazine replaced it starting in 1972."
- [Alumnus Digital Collection](http://archives.nd.edu/Alumnus/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Bagby Glass Plate Negative Collection

From the [University Archives](http://archives.nd.edu/digital/):
- "The Bagby company, a South Bend photographic studio, took pictures of athletes for Notre Dame. The digitized Glass Plate Negative Collection is part of a [larger Bagby collection](http://archives.nd.edu/findaids/ead/xml/bby.xml)."
- [Bagby Glass Plate Negative Collection (Notre Dame Sports), 1920s-1930s](http://archives.nd.edu/Bagby/index.htm/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Annual Bulletins and Catalogs

From the [University Archives](http://archives.nd.edu/digital/):
- "Notre Dame's catalogues or bulletins included descriptions of courses, programs, curricula, facilities, and faculty. They generally [listed students](http://archives.nd.edu/bulletin/stdnts.htm) and provided information on [graduation ceremonies](http://archives.nd.edu/bulletin/cmmncmts.htm), degree recipients, and academic prizes won by students."
- [Notre Dame Annual Catalogues or Bulletins, 1850 - 1914](http://archives.nd.edu/bulletin/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Capstan

From the [University Archives](http://archives.nd.edu/digital/):
- "During World War II, the United States Navy trained many officers at Notre Dame. The naval program published its own yearbook, called Capstan."
- [Capstan, 1943-1945, Digital Collection](http://archives.nd.edu/Capstan/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Commencement Programs

From the [University Archives](http://archives.nd.edu/digital/):
- "Programs for graduations at the University of Notre Dame. The number of commencements per year varies. The content of programs also varies, but they generally provide information about graduating students, speakers, related events and ceremonies."
- [Notre Dame Commencement Programs, 1845 - 2018](http://archives.nd.edu/Commencement/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Daily

From the [University Archives](http://archives.nd.edu/digital/):
- "The Notre Dame Daily first appeared on the twentieth of May, 1923. It published thirteen issue in its first volume, concluding at the end of the academic year on the sixth of June. Its second and final volume covered the 1923-1924 academic year in 128 issues beginning on the twenty-third of September and ending on the fifteenth of June."
- [Notre Dame Daily (student newspaper), 1923 - 1924](http://archives.nd.edu/Daily/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Directories

From the [University Archives](http://archives.nd.edu/digital/):
- "Lists of Notre Dame officers, administrators, rectors, prefects, faculty, post-doctoral research fellows, and students. The alphabetical list of faculty generally indicates academic department, campus address and home address. The alphabetical list of students gives major subject or academic program, dorm or local address, and home address."
- [Notre Dame Directories, 1922 - 1974](http://archives.nd.edu/dir/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Magazine

From the [University Archives](http://archives.nd.edu/digital/):
- "The Notre Dame Foundation published this quarterly magazine, which includes much of general interest to anyone studying Notre Dame in the middle of the twentieth century."
- [Notre Dame: A Magazine, 1948-1965](http://archives.nd.edu/ndm/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Observer

From the [University Archives](http://archives.nd.edu/digital/):
- "The Observer started providing news for the University of Notre Dame and Saint Mary's College starting in the fall of 1966, first as a weekly, then bi-weekly, and soon as a daily newspaper. Starting with the issue of October 10, 2009, the Notre Dame / Saint Mary's Observer appeared online (http://ndsmcobserver.com/)."
- [The Observer (student newspaper), 1966 - 2015](http://archives.nd.edu/Observer/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Scholastic

From the [University Archives](http://archives.nd.edu/digital/):
- "The Scholastic, a student weekly, began in 1867 as The Scholastic Year. For most of its history it provided news about Notre Dame as well as feature articles, literary works, essays, and alumni notes."
- [Notre Dame Scholastic (student magazine), 1867 - 2011](http://archives.nd.edu/Scholastic/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Scholastic Football Review

From the [University Archives](http://archives.nd.edu/digital/):
- "The Notre Dame Scholastic published reviews of the football season starting in 1901. In 1910 a separate publication covered the "Gridiron Season" and from 1919 to 1921 a Football Review provided competition for the Scholastic. From 1924 to 1932 the Football Review prevailed as the Scholastic provided little or no commentary. In later years the Scholastic generally published its own special issue on the football season, though Irish Eye took over for a time in the 1980s."
- [Notre Dame Football Review, 1901 - 2010](http://archives.nd.edu/Football/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

### Voice

From the [University Archives](http://archives.nd.edu/digital/):
- "The Voice of Notre Dame, predecessor of the more familiar daily Observer, appeared somewhat irregularly every week or so between 1963 and 1966, though issues were sometimes printed as little as two days apart."
- [Notre Dame Voice (student newspaper), 1963 - 1966](http://archives.nd.edu/Voice/)

Google Drive:
- [Files](https://drive.google.com/drive/folders/1EILKXMGwZawvZbuAhOZkSNfK9JnqOEr_?usp=sharing)
- [Metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

## Next Steps: Metadata

Once you've selected materials to work with, you'll need to build out metadata for the static site platform and Omeka.

Prof. Walden has created metadata templates for each platform, and pulled starter metadata (URLs, file names, object descriptions) from the ND Archives.

Google Drive:
- [Metadata templates](https://drive.google.com/drive/folders/1NuVx0qiOBahf0neMnT9RYF_VlwkgiiVv?usp=sharing)
- [Folder with starter metadata](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing)

Copy what you need into your group's Google Drive folder (or create shortcuts) and build out two metadata files:
- Static site (Wax or Collection Builder)
- Omeka

## Next Steps: Technical Infrastructure

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

### Static Sites

Note on scope: You're not being asked to develop a full-scale functioning project here. Folks working on this task should expect to spend 1-2 hours working on the static site you're buliding.

At this point, the person who is the GitHub wrangler or point person for your group should have made a copy (fork) of a repository for the platform you're using and have gone through the necessary software installs.

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

#### Collection Builder

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

### Omeka

Note on scope: You're not being asked to develop a full-scale exhibit here. Folks working on this task should expect to spend 1-2 hours working on building metadata for a collection of materials.


Step 1: [Copy Omeka metadata template](https://docs.google.com/spreadsheets/d/1dMWU5a2xe6S4vVjNUrsXXVETJkdj8gH0xfEi6Cuk5VU/edit?usp=sharing)

Step 2: If needed, take a look at [sample Omeka metadata](https://drive.google.com/drive/folders/1dU2jGfitJkLn6XOmCRglXIYu0QnnZs4P?usp=sharing)

Step 3: [Add the existing metadata for your collection](https://drive.google.com/drive/folders/1Cl4d22PQgJd6wKsjNq3W2mxGA01QZK3F?usp=sharing) to your copy of the Omeka template
- Directories (Christian, Juan)
- Magazine (KMCPLC)
- Observer (Audrey, Sydney, Kelly, Chris, Amy)
- Scholastic (Jack Coan)
- Voice (Charlotte, Grace, Maura, Carolyn, Caitlyn)

Step 4: Fill out the rest of the metadata template ([more documentation on metadata fields](https://omeka.org/classic/docs/Content/Working_with_Dublin_Core/))

Step 5: Send metadata file to Prof. Walden
- Or, if you want to create the collection in Omeka yourself...
  * Log in to Omeka Sandbox site using your ND email ([public site](http://kwaldenphd.com/omeka-classic-sandbox/), [admin login](https://github.com/kwaldenphd/football-exhibits/blob/main/kwaldenphd.com/omeka-classic-sandbox/admin)
  * [Create a collection](https://omeka.org/classic/docs/Content/Collections/)
  * [Import using `CSV Import` plugin](https://omeka.org/classic/docs/Plugins/CSV_Import/)

Step 6: Head to http://kwaldenphd.com/omeka-classic-sandbox/ to check out your collection!

## While You're Working on All of That...Task #3

The last thing you're asked to do is build a small-scale immersive/interactive digital story.
- Note on scope: You're not being asked to develop a full-scale research project here. Folks working on this task should expect to spend 1-2 hours working on whatever you're building.
- Folks can work collaboratively on the same project or work individually with different tools. 

Step 1: The first step is figuring out what platform(s) or tool(s) you want to explore and what you're interested in building.

Options include:
- Adobe Spark
- ArcGIS StoryMaps
- Timeline JS
- Storymap JS
- Storyline JS
- CurateScape (built on Omeka- Prof. Walden has a sandbox site already created. Let her know if you want to be added)
- Something open-source/homegrown
- If you want to dabble in 360/VR/AR/MR
  * StorySphere
  * SceneVR
  * Etc

Step 2: Once you've nailed that down, you might need to build out things like...
- Object inventory
- Design/visual content
- Text
- Interactive map(s)
- Metadata

Tutorials:
- [Adobe Spark](https://remix.nd.edu/photo-essay.html)
- [TimelineJS](https://remix.nd.edu/interactive-timeline.html)
- [StorymapsJS](https://lindseywieck.org/fall_2016_sf/storymapjstutorial.html)
- [ArcGIS StoryMaps](https://github.com/kwaldenphd/ArcGIS-StoryMaps)
- CurateScape
  * [CurateScape documentation](https://curatescape.org/docs/content-creation-guide/)
  * [University of Oregon Library Guide](https://researchguides.uoregon.edu/c.php?g=900917&p=6482491)

Step 3: Publish your project and share link as part of lab notebook.

## Lab Notebook Components

- Reflections/observations from the Background section of the lab
- Reflections/observations from the Metadata section of the lab
- Reflections/observations from your work exploring tools and sample projects
- Your group's work building out digital exhibit/archive and immersive/interactive digital story
  * Any data files you worked with
  * Public-facing things you created (GitHub Pages site, Omeka collection/exhibit, StoryMap, timeline, etc)
- Individual reflection
  * At least 200 words (or 2-3 minutes audio/video), addressing the following questions:
    * What you learned about metadata through this lab
    * What you learned about digital exhibits/archives through this lab
    * What you learned about immersive/interactive digital storytelling through this lab
    * How you're thinking about these tools/approaches as they relate to ND football history and primary sources differently after this lab
    * Where you would go next with these tools/methods (other research questions/topics you're interested in exploring, other data sources or types of data you would want to be able to work with, etc)
    * Other comments/questions/observations

If you're working in Google Drive, you can just submit a link to Google Drive.

Notebooks can be individual or collaborative.
