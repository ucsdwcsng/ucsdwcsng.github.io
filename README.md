## How to Update WCSNG Website
### Home Page
To update the images in the carousel, go to index.md and update the image paths under the carousels in the fronnt matter.   
To change the research areas or their overview gifs, update the coressponding heading, link, and path in the body of index.md.
For now, these research areas are hardcoded, but it could be automated if they change a lot by creating a .yml file.
### Team Page
To update current PhD students, Postdocs, or Collaborators, add (or remove) an entry in /_data/people.yml. Be sure to follow the same format as the existing entries with name, role, and a path to their image. Thes images should be saved to /assets/images/teampic.   
To update current Masters and Undergraduate students, add (or remove) an entry in /_data/people_text.yml. Again, be sure to follow the same format as the existing entries. For the `col` field, alternate 1 and 2 for each additional entry to make sure that the names are evenly split across both columns.   
To update Alumni, add (or remove) an entry in /_data/alumni.yml. Be sure to alternate the col values for each entry, as described above. For the `role` field, put the degree for all alumni (BS, MS, PhD etc.). For the `year` field, put the graduating year for all alumni. The `now` field can be left empty if unknown, or phrased " [company] [location]" or "[degree] at [school]".
### Research Pages
To add a new research page, create a new md file and put `layout: research` in the front matter. Add the `pubtag` field to indicate which publications to display on the list of that research page. Be sure to match the spelling exactly to the corresponding tag on the publications. The `heading` field should have the title of the research page (it is not `title` for this layout since we want to display it below the research navbar). The `people` field is a list of the phd and postdoc students involved in this research area. Add them in the following format, and the layout will automatically pull their images from the people.yml file:
```
people:
  - Dinesh Bharadia
  - Roshan Ayyalasomayajula
  - Ish Kumar Jain
  - Aditya Arun
  - Wei Sun
  - Deepak Vasisht
  - Shunsuke Saruwatari
  - Chi Zhang
```
The `sponsors` field is optional, and should include a list of sponsors and their logos in the following format:
```
sponsors:
  - name: Qualcomm
    picture: /assets/images/qualcomm.jpeg
```
Finally, use the `carousels` field to add the research page's carousel images using the following format:
```
carousels:
  - images:
    - image: /assets/images/atkinson.jpeg
    - image: /assets/images/rice_chip.jpeg
    - image: /assets/images/pcb.jpeg
    - image: /assets/images/bearl.jpeg
```
### Publications
To add a new publication (both to the publications list and as an individual webpage), create a new md file under /_posts. Be sure to name the md file with the format `year-month-day-name.md` (ex: 2023-05-24-mmSpoof.md). In the front matter of this md file, add `layout: publication`. The `title` field should have the full name of the publication, which will be displayed as the title of the publication's webpage. The `short_title` field is the shortened name that will be displayed on the list views of the publication. The `tags` field is a space separated list to tag which sublists and research pages this publication should appear in. Be very careful to match the spelling exactly to existing tags, or it will create a new tag for this publication. The `cover` field should have the path to the cover image to be displayed on the publication list. All cover images should be saved to /assets/images/pubpic. The `authors` field should be a string of authors separated by commas (try to write full names and only commas, no "and" to maintain consistency). The `conference` field stores the name of the conference this paper was used in. The `paper` field is required, and should contain a link or path to a pdf of the paper. Most of these pdfs are stored in /files. The optional fields are `github`, which should have a link to the github repo, `dataset`, which should have a link the the dataset, `slides`, which should have a path to a pdf of the slides (most are saved in /files), `extra`, which should have a string about the special highlight of this publication (ex: `extra: "This work won the Qualcomm Innovation Fellowship 2022!"`), and `video`, which should have an EMBED link to a youtube video (not the regular youtube link). Currently, up to two video links are automatically supported, with the field for the second video being `video2` (which will also require a youtube embed link). Up to one additional link is also supported under the field `other`, which will show up in the list of links containing the slides, github, and datasets. The format for adding this extra link is:
```
other:
  display: "[Kaggle Competition]"
  url: https://www.kaggle.com/competitions/wildv2/data
```
Another optional field is `press` to show any press coverage. Currently, upto 4 press links are supported (with fields `press`, `press2`, `press3`, and `press4`), annd the format to add them is as follows:
```
press:
  date: "November 20, 2020"
  url: https://www.10news.com/news/local-news/uc-san-diego-researchers-find-ways-to-make-self-driving-cars-safer
  headline: UC San Diego Researchers Find Ways to Make Self-Driving cars Safer
```
The `osd` field (named osd as short for Open Source Description - feel free to rename if you can think of a better option) os optional, and should contain a string with a short description of the publication's associated code and/or dataset to be displayed on the Open Source page.
The last optional front matter field is the `highlight` field. This field is a boolean used to determine whether this publication should be one the publications displayed on the shortened list of its corresponding research page. If `highlight` is `true`, then the publication will appear on the shortened research page list. If it is `false`, or the `highlight` field is missing, then it won't.
Finally, the Abstract should be added to the body of the md file. Don't add a heading for the abstract, since that formatting is already automated by the publication layout. Any customized headings, images, and videos can also be added in the body, and will be displayed below the abstract on the webpage.
The publication list will display icon links for any provided github, slides, and paper, but not any of the other optional fields. The other optional fields will be viewable on the publications webpage, which will be accessible by clicking the title on the publications list, or the shortened list on any of the research pages.
