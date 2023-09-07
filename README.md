<h2>How to Update WCSNG Website</h2>
<h3>Home Page</h3>
To update the images in the carousel, go to index.md and update the image paths under the carousels in the fronnt matter.   
To change the research areas or their overview gifs, update the coresspoonding heading and path in the body of index.md.
<h3>Team Page</h3>
To update current PhD students, Postdocs, or Collaborators, add (or remove) an entry in /_data/people.yml. Be sure to follow the same format as the existing entries with name, role, and a path to their image. Thes images should be saved to /assets/images/teampic.   
To update current Masters and Undergraduate students, add (or remove) an entry in /_data/people_text.yml. Again, be sure to follow the same format as the existing entries. For the `col` field, alternate 1 and 2 for each additional entry to make sure that the names are evenly split across both columns.   
To update Alumni and Interns, add (or remove) an entry in /_data/alumni.yml. Be sure to alternate the col values for each entry, as described above. For the `role` field, put the degree for all alumni (BS, MS, PhD etc.), and the program for interns (SRIP or Intern). The International Summer Intern entries have an extra field `school` to store which school they are originally from. For the `year` field, put the graduating year for all alumni and the internship year for all interns. The `now` field can be left empty if unknown, or phrased "Now at [job] [location]" or "Now [degree] at [school]".
<h3>Research Pages</h3>
To add a new research page, create a new md file and put `layout: research` in the front matter. Add the `pubtag` field to indicate which publications to display on the list of that research page. Be sure to match the spelling exactly to the corresponding tag on the publications. Add the carousel images to the front matter using the following format:
'''
carousels:
  - images:
    - image: /atkinson.jpeg
    - image: /rice_chip.jpeg
    - image: /pcb.jpeg
    - image: /bearl.jpeg
'''
<h3>Publications</h3>
To add a new publication (both to the publications list and as an individual webpage), create a new md file under /_posts. Be sure to name the md file with the format `year-month-day-name.md` (ex: 2023-05-24-mmSpoof.md). In the front matter of this md file, add `layout: publication`. The `title` field should have the full name of the publication. The `tags` field is a space separated list to tag which sublists and research pages this publication should appear in. Be very careful to match the spelling exactly to existing tags, or it will create a new tag for this publication. The `cover` field should have the path to the cover image to be displayed on the publication list and header of the publication page. All cover images should be saved to /assets/images/pubpic. The `authors` field should be a string of authors separated by commas (try to write full names and only commas, no "and" to maintain consistency). The `conference` field stores the name of the conference this paper was used in. The `paper` field is required, and should contain a link or path to a pdf of the paper. Most of these pdfs are stored in /files. The optional fields are `github`, which should have a link to the github repo, `dataset`, which should have a link the the dataset, `slides`, which should have a path to a pdf of the slides (most are saved in /files), `highlight`, which should have a string about the special highlight of this publication (ex: `highlight: "This work won the Qualcomm Innovation Fellowship 2022!"`), `video`, which should have an EMBED link to a youtube video (not the regular youtube link). Currently, up to two video links are automatically supported, with the field for the second video being `video2` (which will also require a youtube embed link). Up to one additional link is also supported under the field `other`, which will show up in the list of links containing the slides, github, and datasets. The format for adding this extra link is:
'''
other:
  display: "[Kaggle Competition]"
  url: https://www.kaggle.com/competitions/wildv2/data
'''
Another optional field is `press` to show any press coverage. Currently, upto 4 press links are supported (with fields `press`, `press2`, `press3`, and `press4`), annd the format to add them is as follows:
'''
press:
  date: "November 20, 2020"
  url: https://www.10news.com/news/local-news/uc-san-diego-researchers-find-ways-to-make-self-driving-cars-safer
  headline: UC San Diego Researchers Find Ways to Make Self-Driving cars Safer
'''
Finally, the Abstract should be added to the body of the md file. Don't put an abstract heading, since that formatting is already automated by the publication layout. Any customized headings, images, and videos can also be added in the body, and will be displayed below the abstract on the webpage.
The publication list will display icon links for any provided github, slides, and paper, but not any of the other optional fields. The other optional fields will be viewable on the publications webpage, which will be accessible by clicking the title on the publications list, or the shortened list on any of the research pages.