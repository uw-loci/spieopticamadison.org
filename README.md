# Editing Fundementals

To make edits to this website, you'll need a [GitHub Account](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account) and access to this repository. See instructions here for how to [apply 2FA to your GitHub account](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa).

### Add, edit, upload files
Instructions for making changes to an exisiting file, e.g. the homepage: `/pages/index.md`: [edit an exisiting file](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files)

Instructions for creating a new file, e.g. a new event or news page: [create a new file](https://docs.github.com/en/repositories/working-with-files/managing-files/creating-new-files)

Instructions for uploading a file, e.g. an image: [upload a file](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)


### Markdown Syntax
Github pages content is written in markdown syntax, see a guide [here](https://www.markdownguide.org/basic-syntax/).

Here are some common kinds of text formatting in markdown:

| Formatting                               | Markup                                     |
|------------------------------------------|--------------------------------------------|
| *italic text*                            | `*italic text*`                            |
| **bold text**                            | `**bold text**`                            |
| ***bold and italic text***               | `***bold and italic text***`               |
| `fixed width text/code`                  | <code>`fixed width text/code`</code>       |
| ~~struck-out text~~                      | `~~struck-out text~~`                      |
| [Hyperlink](https://example.com/)        | `[Hyperlink](https://example.com/)`        |
| <span style="color: red">red text</span> | `<span style="color: red">red text</span>` |

# News, Events, and Leader Profiles
The UW-Madison SPIE/OPTICA chapter executive board is responsible for updating three main components of this website:
1) Events
2) News
3) Leadership

# Creating an event page
1) Create a new file in `/_pages/events`
2) Create a file name in the format `YYYY-MM-DD-short-description.md`, NOTE:
    - files MUST begin with the date format `YYYY-MM-DD-` to be parsed by the events list.
    - files MUST end with `.md` to be read as content by github pages.

3) Set your frontmatter. Frontmatter is a list of varibles set at the start of the page. For the events listing, you MUST set the following frontmatter:
    - title: The title you want displayed on the event page, can be different from the filename and can include whitespace.
    - day: the date of the event, in format: `Month DD, YYYY` e.g. November 13, 2022
    - time: the time of the event, format: 3 PM, 1:30 PM, 4 AM, etc
    - image: the filename of your chosen event image, e.g. `my-image.png`
    - image-description: text description of your image, this is an accessbility feature

Feel free to copy/paste the code snippet below and fill in content for your new event. Frontmatter must be sandwiched between ```---```.
```
---
title: My Event Name
day: Month DD, YYYY
time:  PM
image: speaker-image.png
image-description: picture of speaker
---
```
4) Fill in the body content of your page after the front matter.
5) Place your image file in the following folder: `/assets/images/events`. Image files placed elsewhere will not populate in the events listing.

# Creating a News page

1) Create a new file in `/_pages/news`
2) Create a file name in the format `YYYY-MM-DD-short-description.md`, NOTE:
   - files MUST begin with the date format `YYYY-MM-DD-` to be parsed by the events list.
   - files MUST end with `.md` to be read as content by github pages.

3) Set your frontmatter. Frontmatter is a list of varibles set at the start of the page. For the events listing, you MUST set the following frontmatter:
   - title: Unlike events, news page titles MUST be in the format `YYYY-MM-DD shortdescription`, but can still include whitespace.

Feel free to copy/paste the code snippet below and fill in content for your new news page. Frontmatter must be sandwiched between ```---```.
```
---
title: YYYY-MM-DD my news listing
---
```
4) Fill in the body content of your page after the front matter.

# Creating a leadership page
Currently, SPIE has 5 officers and a faculty advisor. These listings will need to be updated as members of the executive committee come and go. To swithc out a member:
1) Delete/remove the outdated officer page in `/_pages/leadership/`
2) Place the head shot image of the new officer in `assets/images/leadership`
3) Create a new page in `/_pages/leadership` in format `lastname.md`
4) Set your frontmatter. Frontmatter is a list of varibles set at the start of the page. For the events listing, you MUST set the following frontmatter:
   - title: Full name of the new member/officer, can include whitespace
   - role: e.g. "Vice-President, Communications Officer, Treasurer, Faculty Advisor, etc.
   - image: the filename of the new officer image, e.g. `lastname.png`
   - image-description: text description of your image, this is an accessbility feature
   - order: a numerical value, controls the order of the leadership listing 1 being first, 6 being last

Feel free to copy/paste the code snippet below and fill in content for your new leadership page. Frontmatter must be sandwiched between ```---```.
```
---
title: Firstname Lastname
role: Vice-President
image: lastname.png
image-description: Photo of Firstname Lastname
order: 2
---
```
5) No body content is required for leadership pages
