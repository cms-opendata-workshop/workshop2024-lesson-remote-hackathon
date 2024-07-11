# The Carpentries Workbench Template Markdown Lesson

This lesson is a template lesson that uses [The Carpentries Workbench][workbench]. 

## Note about lesson life cycle stage
Although the `config.yaml` states the life cycle stage as pre-alpha, **the template is stable and ready to use**. The life cycle stage is preset to `"pre-alpha"` as this setting is appropriate for new lessons initialised using the template.

## Create a new repository from this template

To use this template to start a new lesson repository, 
make sure you're logged into Github.   
Visit https://github.com/cms-opendata-workshop/workbench-template-md/generate
and follow the instructions.
Checking the 'Include all branches' option will save some time waiting for the first website build
when your new repository is initialised.

If you have any questions for DPOA, ask on Mattermost!. If you have any questions for the carpentries developer, contact [@tobyhodges](https://github.com/tobyhodges)

## Configure a new lesson

Follow the steps below to
complete the initial configuration of a new lesson repository built from this template:

1. **Make sure GitHub Pages is activated:**
   navigate to _Settings_,
   select _Pages_ from the left sidebar,
   and make sure that `gh-pages` is selected as the branch to build from.
   If no `gh-pages` branch is available, check _Actions_ to see if the first
   website build workflows are still running.
   The branch should become available when those have completed.
1. **Adjust the `config.yaml` file:**
   this file contains global parameters for your lesson site.
   Individual fields within the file are documented with comments (beginning with `#`)
   At minimum, you should adjust all the fields marked 'FIXME':
   - `title`
   - `created`
   - `keywords`
   - `life_cycle` (the default, _pre-alpha_, is the appropriate for brand new lessons)
   - `contact`
1. **Annotate the repository** with site URL and topic tags:
   navigate back to the repository landing page and
   click on the gear wheel/cog icon (similar to ⚙️) 
   at the top-right of the _About_ box.
   Check the "Use your GitHub Pages website" option,
   and [add some keywords and other annotations to describe your lesson](https://cdh.carpentries.org/the-carpentries-incubator.html#topic-tags)
   in the _Topics_ field.
   At minimum, these should include:
   - `lesson`
   - the life cycle of the lesson (e.g. `pre-alpha`)
   - the human language the lesson is written in (e.g. `deutsch`)

## Notes for CMS Open Data lessons

No attempt for a local build was made, and in principle, there is no need to install R or Pandoc. Note, however, that the content should be in [Pandoc-flavored Markdown](https://pandoc.org/MANUAL.html). If one wishes to test locally, the instructions are provided in [The Carpentries Workbench][workbench] documentation.

The setup instructions are in `learners/setup.md` and the separate pages under `episodes`.

The `md-outputs` branch shows after setting up the repository. No need to merge them.

The schedule shows only in the "Instructor view": https://cms-opendata-workshop.github.io/workshopqcd-2024-lesson-docker/instructor/index.html 
Use this link if you want to show it.

### Updating an old lesson to the new template

There might be a tool somewhere, but if doing it by hand:

1. Change questions (note the empty line after items), objectives and keypoints to
   ```
   :::::: questions
   - question 1
   - question 2

   ::::::

   :::::: objectives
   - objective 1
   - objective 2

   ::::::

   <!-- EPISODE CONTENT HERE -->

   :::::: keypoints
   - keypoint 1
   - keypoint 2
   ::::::
   ```
2. Remove the double quotes of the question, objectives and keypoints.
3. Make sure that keypoints are at the end of the text.
4. Find all `{: .callout}`, `{: .challenge}`, `{: .testimonial}` etc tags and and remove the preceeding `> ` for the block and change them to

   ```
   ::: callout
   This is a callout block. It contains at least three colons
   :::
   ```
   or

   ```
   ::::::::::::::::::::::::::::::::::::: challenge

   ## Question

   Q: question

   :::::::::::::::: solution

   A: answer

   :::::::::::::::::::::::::
   :::::::::::::::::::::::::::::::::::::::::::::::
   ```

### Documentation

See e.g.

- https://carpentries.github.io/lesson-development-training/
- https://carpentries.github.io/sandpaper-docs/index.html

### Indents and unexpected code blocks

Note that double-indent (two tabs) or anything more that three spaces produces a code block. That's not necessarily what one would expect.
Also, in some special cases, in nested lists, the second level items might appear as a code block.
 
### Figures

Figures should be located under `episodes/fig`, and included, for example, with

```
![](fig/portal_screenshot_landing_page.png)
```


[cff-home]: https://citation-file-format.github.io/
[cff-sandpaper-docs]:  https://carpentries.github.io/sandpaper-docs/editing.html#making-your-lesson-citable
[cffinit]: https://citation-file-format.github.io/cff-initializer-javascript/
[workbench]: https://carpentries.github.io/sandpaper-docs/
