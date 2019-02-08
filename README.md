# Yu Lab Website

This is the website of the Yu Lab academic research group at Stowers Institute for Medical Research.

This website is powered by Jekyll and some Bootstrap, Bootwatch. This website hails from the Allan Lab (Leiden University), who generously shared their codebase and invited others to use their design as a basis for their own websites.

Code released under the MIT License.

---
---

# Updating the lab website

Jekyll is a blog-aware, static site generator written in Ruby. In brief, you create a bunch of flat files (meaning: no database) and the Jekyll engine generates HTML based on those files. In other words, create content (usually in markdown), create a template page to show that content, and the compiler engine will generate HTML webpages.

Github is kind enough to host the site for free, as well as generate the HTML webpages from the content files on the fly. This means we can update the website without ever downloading a file. Everything can be done using Github's text editor and web uploader for images.

For the most part, you can reproduce what already exists, like using an existing team member's `.yml` chunk and modifying the details.


# Relevant folders

## _data folder

Here is where you'll do most of the maintenance. Other parts of the website shouldn't be changing as frequently as these parts. You'll edit lab member information, add new publications, add news, and allow pictures to be displayed on the **Pictures** page.

## _pages folder

Here you'll modify the job postings in `opportunities.md` the research direction/background in `research.md`, and the alumni information in `team.md`. See the explicit walkthroughs below for info on how to manipulate information in these.

## images folder

All of the images live in this folder. When you want to include an image in a post or alongside a team_member tile you'll be able to proved the path to where the image resides. The folder structure is for organization only. If you want to change the name of an existing folder you'll have to be thorough with updating the paths referencing the original path, so it'll be easiest to leave them as they are and to follow the existing scheme.

# Specific tasks

## Updating current lab member information

Each person has a little YAML chunk that looks like:

```
- name: Kohl Kinning
  photo: kohl_kinning.jpg
  info: Bioinformaticist
  email: kkinning@stowers.org
  number_educ: 2
  education1: B.A. Biology, Lewis and Clark College
  education2: M.Sc. Biology, University of Oregon
```

This can be edited and saved through the Github user interface and the changes will be automatically applied to the site. There are different files for different categories of lab members. The text above can be found in `_data/team_members.yml`. You'll see different categories like *PhD Students*, *Graduate Researchers*, and so on. The image for each person should be added to `images/teampic` and should be referenced as in the example above.

![](/images/tutorialpic/editing_team_members.png)

# Adding alumni

This part is not optimal and editing raw HTML is necessary. At line 299 is where the alumni section begins. For each `<tr></tr>` chunk, there is an entry for Postdoctoral Research Associates, Research Technicians, and Graduate Researchers. So Jie He was a Postdoctoral Research Associate, Evan Gillespie was a Research Technician, and Vasha DuTell was a Graduate Researcher. This will be changed soon so that you can just add a name to a `.yml` file under `_data` and this section will be updated.

![](/images/tutorialpic/editing_alumni.png)

# Adding pictures

This is a two step procedure:

1. Upload the image with the Github user interface. Navigate to the correct folder and click `Upload files` in the top right corner.
2. Depending on where you will be using the image, update the the intended location of the image with the path
  + if it's going to be associated with any thing in the `_data` folder, just provide the filename e.g. `kohl_kinning.jpg`
  + if it's on a page in the _pages folder you have to place this Markdown/HTML blend where you want the image `![]({{ site.url }}{{ site.baseurl }}/images/foldername/filename.png){: style="width: 30%; float: center; border: 10px"}`
  + if it's abreast a news item, place this after the text (on the same line) `<img src='/images/newspic/sfn_2018.jpg' class='img-responsive' style='max-width: 192px' />"`
  
 # Adding a News item to the homepage
 
Navigate to `_data/new.yml` and follow the formatting of the other items. Add the newest item to the top of the list. YAML is very picky about syntax (whitespace, colons, etc) so be mindful of using the scaffolding of the other news entries. This section would ideally be be replaced by a Twitter widget.
