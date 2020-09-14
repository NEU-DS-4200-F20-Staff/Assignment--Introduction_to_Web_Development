# Assignment — Introduction to Web Development

This repository is your starting point for the assignment and includes the instructions below. 

Link to GitHub pages website: `[insert your hyperlink here]`


## Aim of the Assignment:

In this assignment you will work through several examples and resources on the Mozilla Developer Network (MDN) in order to learn the basics of web development and using HTML, CSS, JavaScript,  git, GitHub, and GitHub Pages. This will complement an in-class activity in Lecture 2 where we use these technologies.

**_If you struggle a lot on this assignment or feel lost, seek additional web development training outside of class ASAP and come to office hours for help._** One goal of this assignment is to help you realize what you may need to learn. We will be doing some instruction in class but we expect that many of you will need to use tutorials and other outside resources to accomplish the upcoming assignments.


## Instructions:

Work through the [MDN Getting Started with the Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web) module.

First, get your GitHub repository you will be using for the assignment by following the GitHub Classroom invitation link in the assignment on Canvas.

Then work through the following sections, links, and steps:

1. [Installing basic software](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/Installing_basic_software)
    *   Web browser: We recommend [Firefox](https://www.mozilla.org/en-US/firefox/new/) or [Chrome](https://www.google.com/chrome/)
    *   Graphics Editor: We recommend [GIMP](https://www.gimp.org/)
    *   Version control system: We are using [Git](https://git-scm.com/) and [GitHub classroom](https://classroom.github.com/). On Windows, [TortoiseGit](https://tortoisegit.org/) provides a nice user interface to Git.
    *   ~~An FTP program: Isn't needed for this assignment.~~
    *   ~~An automation system: Isn't needed for this assignment.~~
    *   [Install Python to use a local web server](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server). You may already have Python installed. If you are using Python 2 please switch to Python 3 as [Python 2 was sunset on 2020-01-01](https://www.python.org/doc/sunset-python-2/).

1. Clone this repository to your local machine.

    E.g., in your terminal / command prompt `CD` to where you want this the folder for this activity to be. Then run: `git clone <YOUR_REPO_URL>`

    **Under no circumstances should you be editing files via the GitHub website user interface.** Do all your edits locally after cloning the repository.

1. [What will your website look like?](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/What_will_your_website_look_like)
    
    Don't worry about sketching or finding an image. We provide the images for you in your git repo in the `images` folder.
    
1. [Dealing with files](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/Dealing_with_files)
    
    We provide a basic website structure in your git repo. Please edit the included files:
    * `README.md` is this explanatory file for the repo.
    * `index.html` will contain the main HTML website content.
    * `styles/main.css` will contain the CSS.
    * `scripts/main.js` will contain the JavaScript.
    * `LICENCE` is your source code license.

1. [HTML Basics](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/HTML_basics)

    **Commit and push your files to GitHub after this step.**
    
    E.g., `git add *` then `git commit -m "My commit message"` followed by `git push --all origin`.

1. [CSS Basics](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/CSS_basics)

    **Commit and push your files to GitHub after this step.**

1. [JavaScript basics](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/JavaScript_basics)
    
    Also work through [What are browser developer tools?](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools), including the details for your particular browser. Note that using Chrome or Firefox will work better for this course.
    *   [Firefox Page inspector](https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector)
    *   [Chrome DOM inspector](https://developer.chrome.com/devtools/docs/dom-and-styles) (Opera's inspector works the same as this)
    *   [Safari DOM inspector and style explorer](https://developer.apple.com/library/safari/documentation/AppleApplications/Conceptual/Safari_Developer_Guide/ResourcesandtheDOM/ResourcesandtheDOM.html#//apple_ref/doc/uid/TP40007874-CH3-SW1)
    *   [IE DOM Explorer](http://msdn.microsoft.com/en-us/library/ie/dn255008%28v=vs.85%29.aspx)

    **Commit and push your files to GitHub after this step.**

1. [Publishing your website](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/Publishing_your_website)
    
    * We will use [GitHub pages](https://pages.github.com/). Upon commit (and waiting around 1 min) the web page is served automatically.
    
        You would normally need to turn on GitHub pages in the settings for your repository but we have set that up for you so you're using the `gh-pages` branch by default.

        You can use this JavaScript [bookmarklet](https://en.wikipedia.org/wiki/Bookmarklet) in your browser to swap between any GitHub repository and the associated GitHub Pages site. Create a new bookmark in your browser and copy and paste this code in the `location` field:
        ```js
        javascript: (function() {
        var path = window.location.pathname;
        var ps = path.split("/");
        var f = ps[ps.length - 1];
        var host = window.location.host;
        if (host === "github.com") {
            var repo = path.split('/')[1];
            if ((ps.length === 4 && f === "") || (ps.length === 3)) {
                window.location.href = "http://" + repo + ".github.io/" + path.replace("/" + repo + "/", "")
            } else if (ps.length === 5 || (ps.length === 6 && ps[5] === "")) {
                window.location.href = "http://" + repo + ".github.io/" + ps[2]
            } else if (ps.length > 3 && f.split(".").length === 2) {
                var newpath = path.replace("/" + repo + "/", "").replace("blob/gh-pages/", "");
                window.location.href = "http://" + repo + ".github.io/" + newpath.replace(".md", ".html").replace(".Rmd", ".html")
            }
        } else if (host.split('.')[1] === "github" && host.split('.')[2] === "io") {
            var repo = host.split('.')[0];
            if ((ps.length === 3 && f === "") || (ps.length === 2)) {
                window.location.href = "http://github.com" + "/" + repo + path
            } else if (ps.length > 2) {
                var newpath = path.replace(f, "") + "blob/gh-pages/" + f;
                window.location.href = "http://github.com" + "/" + repo + newpath
            }
        }
        })();
        ```
        Then, you can visit a GitHub repository or GitHub Pages site and click the bookmark to swap.

    * Read [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
    *   Edit near the top of your README.md file to include a clickable hyperlink to the GitHub page website for your repo., replacing the `` `[insert your hyperlink here]` `` code with your markdown.
    
    **Commit and push your files to GitHub after this step.**

1. Make any edits necessary to ensure your code passes the [W3 validator](https://validator.w3.org/).

1. Read [How the web works](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/How_the_Web_works).

1. Read [A re-introduction to JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript).


## Submission instructions:

1. Ensure you commit and push your files to GitHub at each step you're instructed to above **in bold**. The steps are: HTML Basics, CSS Basics, JavaScript Basics, Publishing your website.

1. Submit the URL of **your GitHub Classroom-generated repository** to the associated assignment on Canvas. **Do not submit a link to a personal repository. It must be within our class GitHub organization.** 


## Grading:

This is a satisfactory grading assignment. If you followed the instructions you receive full marks and if not you receive a 0. Your submission is satisfactory if:

* Everything is submitted by the due date following the instructions.
    * Any commits made after the due date will be ignored when your work is graded.
    * **If you do not submit the correct link we will not grade your assignment and you will receive a 0**. This is standard course policy.
* Any folders/files are properly named, located as specified, and contain what is expected.
* Your web page link is correctly updated at the top of the README.md file.
* You submit a link to the GitHub Classroom-generated repo, not a personal one.
* Each of the required commits and pushes is done in order and not edited via the GitHub user interface online.
* Your web page loads properly and looks roughly as expected in the latest Firefox and Chrome browsers on the teaching staff's computers.
* Any code from other sources (modified or copied straight) is acknowledged.
* Your submitted code isn't directly copied from Mozilla's repositories and demonstrates that you actually worked through the examples completely.


## Further Reading for those interested:

[MDN Learning HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML)

[MDN Learn to Style HTML using CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)


## Template Repository Setup (For Instructors Only):

### GitHub Pages

It is necessary if using GitHub Classroom to set up GitHub pages for the students, as they do not have admin permissions on their repository. To do this, we need to create and move everything to the `gh-pages` branch and delete the `master` branch.

1. Commit the files to the `master` branch on GitHub.

1. `git branch gh-pages`

1. `git checkout gh-pages`

1. `git branch -D master`

1. `git push origin gh-pages`

1. On GitHub, go to `Settings`->`Branches` and set the default branch to `gh-pages`.

1. `git push origin :master`

### Template Repository

1. On GitHub, go to `Settings` and check the box for `Template repository` at the top. This makes GitHub Classroom copies much faster.