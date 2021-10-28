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
  * [What is metadata?](#what-is-metadata)
  * [Metadata in Action](#metadata-in-action)
  * [Metadata Reflection Questions](#metadata-reflection-questions)
- [Sample Digital Exhibit/Archive Projects](#sample-digital-exhibitarchive-projects)
  *  [Omeka](#omeka)
  *  [Static Sites](#static-sites)
    * [Wax](#wax)
    * [CollectionBuilder](#collectionbuilder)
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
- Goal for the end of 10/28 is to have identified a set of materials you want to work with, have started building out metadata, and have figured out the needed technical infrastructure for the digital archive/exhibit components of the lab
- Goal for the end of 11/4 is to have started piecing things together for the digital archive/exhibit components of the lab and decided on next steps for the immersive/interactive digital story component of the lab

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

IMAGE OF CATALOG CARD

MARC records developed as a way of taking the information represented in a card catalog and moving it into a digital or computer-aided discovery environment.

MARC RECORD IMAGE

While MARC records started as physical punch cards, in the last 30 years, MARC records that functioned as databases continue to evolve and transform via the internet.

SPERBER MARC SCREENSHOT

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


Spin up a working instance of Wax or CollectionBuilder OR substantively modify/expand Prof. Walden's sandbox sites
- Site text
- Metadata
- Pages/configuration

Omeka Exhibit/item group- again, new materials OR substantively modify/expand Prof. Walden's sandbox or starter collections
- Exhibit text
- Metadata
- Exhibit curation/configuration

Immersive/interactive digital story- 
- Adobe Spark
- ArcGIS StoryMaps
- Timeline JS
- Storymap JS
- Storyline JS
- Something open-source/homegrown
- If they want to dabble in 360/VR/AR/MR
  * StorySphere
  * SceneVR
  * Etc

Immersive/interactive components:
- Object inventory
- Design/visual content
- Text
- Potentially interactive maps

## Metadata Reflection Questions

SOMETHING GOES HERE

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

OMEKA PHPMYADMIN IMAGE

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

## Static Sites

In the last few years, advocates of minimal computing principles have been thinking about other ways to create digital archives/exhibits that have less technical overhead than a content management system like Omeka.

Minimal computing is driven by "fundamental questions about choice and necessity," specifically:
- "What do we need?"
- "What don't we need?"
- "What do we want?"
- "What don't we want?"

(Jentery Sayers, "[Miniaml Definitions](http://go-dh.github.io/mincomp/thoughts/2016/10/03/tldr/)" *Minimal Computing Working Group*, 3 October 2016)

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

WAX WORKFLOW IMAGE

https://minicomp.github.io/wiki/assets/wax_workflow.jpeg

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
- [Google Drive]

Image files:
- [GitHub](https://github.com/kwaldenphd/wax-sandbox/tree/main/_data/raw_images/bagby)
- [Google Drive]

### Scholastic Football Review Wax Sandbox

Prof. Walden has also prototyped a Wax site for the [Scholastic Football Review issues from 1901-1931](http://archives.nd.edu/Football/).
- [Public site](https://kwaldenphd.github.io/wax-pdf-sandbox/)
- [GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox)

Again, there are two primary components driving the site: a spreadsheet with metadata and a folder with images created from the original PDFs.

Metadata:
- [GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox/blob/main/_data/scholastic.csv)
- [Google Drive](

Files:
- [GitHub](https://github.com/kwaldenphd/wax-pdf-sandbox/tree/main/_data/raw_images/scholastic)
- [Google Drive](

## CollectionBuilder

Another static site option for digital archives/exhibits is CollectionBuilder.

Developed by librarians at the University of Idaho, "CollectionBuilder is an open source tool for creating digital collection and exhibit websites that are driven by metadata and powered by modern static web technology" ([CollectionBuilder](https://collectionbuilder.github.io/))

From CollectionBuilder's ["About"](https://collectionbuilder.github.io/about.html) page:
<em>
- CollectionBuilder is a lightweight, flexible tool for creating digital collection websites that are driven by metadata and powered by modern static web technology. Using three primary components—a spreadsheet of metadata, a directory of assets, and a configuration file—CollectionBuilder gives information professionals and digital scholarship practitioners agency in building and customizing digital collection websites for free.

- CollectionBuilder is designed and maintained by librarians at the University of Idaho according to the Lib-STATIC approach, a methodology committed to leveraging static-web technologies and librarians’ specialized skills in metadata and classification to create engaging web publications.
</em>

CollectionBuilder uses a combination of Jekyll, GitHub, and Bootstrap for the core website components, and then integrates other open-source libraries (including DataTables, Leafletjs, lightGallery, TimelineJS) to generate other types of visualizations.

COLLECTION BUILDER WORKFLOW IMAGE

https://collectionbuilder.github.io/images/dlf-presentation.jpg

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
- [Google Drive]

Image files:
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-sandbox/tree/main/objects)
- [Google Drive]

### Scholastic Football Review CollectionBuilder Sandbox

Prof. Walden has also prototyped a CollectionBuilder site for the [Scholastic Football Review issues from 1901-1931](http://archives.nd.edu/Football/).
- [Public site](https://kwaldenphd.github.io/collectionbuilder-pdf-sandbox/)
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-pdf-sandbox)

In this case, CollectionBuilder is able to pull the PDF files from URLs that point to where these files exist on the ND Archives website, so the metadata is the primary component for the site and the files are pulled from the URLs.

Metadata:
- [GitHub](https://github.com/kwaldenphd/collectionbuilder-pdf-sandbox/blob/main/_data/scholastic_collectionbuilder.csv)
- [Google Drive](

## Discussion/reflection questions for this section of the lab

SOMETHING GOES HERE



# Sample Digital Exhibits

big bucket categories- how do we take primary sources and present them

Omeka

Static site- Wax and CollectionBuilder

Place-based

CurateScape

Media-rich immersive

Exposure

ArcGIS StoryMaps

Opensource alternatives

Other:
360 immersives
VR/AR/MR
Photogrammetry
3D modeling 


# Next Steps (aka, now it's your turn)

Final project prototype- 

Could be a text analysis extension/continuation from lab #1

Could be taking tools/methods covered in lab #2 and applying/connecting them to new or additional datasets

Could be 

## University Archive Collections

What we've covered so far

Other University Archive

Joyce Sports Collection (RBSC)

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
