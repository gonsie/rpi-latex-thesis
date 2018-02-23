*Just want to get started? See the [rpi-thesis-template](http://github.com/gonsie/rpi-thesis-template) repo!*

# Resources for Writing a Thesis at RPI

The official LaTeX Thesis class file for RPI is maintained by dotCIO and can be found here:

- [thesis.cls](http://www.rpi.edu/dept/arc/docs/latex-thesis/thesis.cls)
- [Thesis LaTeX Preparation page](http://www.rpi.edu/dept/arc/docs/latex-thesis/thesis.cls)

I have made a number of changes to the Thesis class;
**These changes are in no way endorsed by any official at RPI/OGE.**

## Summary of Changes

- Now using Unix line-endings, with no blank spaces at the end of lines
- Commented out the bibentry def.
  Un-comment [line 314](https://github.com/gonsie/rpi-latex-thesis/blob/master/thesis.cls#L314) "for use in making an unnumbered bibliography with hanging indents."
- Added a Candidacy title page (no signature lines).
  Use the command `\softtitlepage`.
- Added command for self attribution footnote. See [template/rpithes.tex:27](https://github.com/gonsie/rpi-latex-thesis/blob/master/template/rpithes.tex#L27) and the OGE Thesis Manual (page 12).
  This requires that line [thesis.cls:314](https://github.com/gonsie/rpi-latex-thesis/blob/master/thesis.cls#L314) be commented out.

# Usage of This Repository

This repository is a collection of resources for students writing RPI theses.

## Thesis TeX Style File

The main resource is the TeX style-file, `thesis.cls`.
This is the main file, and really, the only one you need to get started.
A link to the original file and a list of changes is noted above.

## RPI's Provided Template

The files in the `template` folder contain the RPI thesis template tex files (originally provided by dotCIO).

There are two changes:
1. In [rpithes.tex:32](https://github.com/gonsie/rpi-latex-thesis/blob/master/template/rpithes.tex#L32) for the self attribution required by the OGE Thesis Manual (page 12).
2. In [rpithes.tex:15](https://github.com/gonsie/rpi-latex-thesis/blob/master/template/rpithes.tex#L15) for automated figure caption placement below the figure, and table caption placement above the figure. As well as caption bolding and centering.

## RPI/OGE Forms

Hard copies of some of the needed forms can be found in the `OGE-forms` folder.

- RPI's Office of Graduate Education for Current Students: http://gradoffice.rpi.edu/update.do?catcenterkey=2
  - see right-hand sidebar for links to forms and checklists
- RPI's Academic Calendar: http://www.rpi.edu/academics/calendar
  - includes thesis/dissertation due dates
  - includes deadlines for defences
- Offical Thesis/Dissertation guides: https://info.rpi.edu/graduate-academics/submit-your-thesis-dissertation
  - includes guidelines for citing your own work
  - includes document style/formatting specifications
- dotCIO Thesis Page: http://dotcio.rpi.edu/services/printing-publishing/thesis-preparation
  - includes original LaTeX and MSWord templates

## Pro Tips!

Over the years, many students have had difficulties in having their theses accepted by OGE.
In an attempt to alleviate this process, several individuals have passed on their wisdom.
These pro-tips can be found in the `tips` folder, including:

- [ThesisFormatting.md](https://github.com/gonsie/rpi-latex-thesis/blob/master/tips/ThesisFormatting.md): This file lists several reasons why a thesis was returned to a student.
- [Medha_Atre_Comments.md](https://github.com/gonsie/rpi-latex-thesis/blob/master/tips/Medha_Atre_Comments.md): This file contains Medha's comments on the thesis submission process, as emailed to the CSGrads list in September 2011.
- [Terry_Hayden_Pro_Tips.md](https://github.com/gonsie/rpi-latex-thesis/blob/master/tips/Terry_Hayden_Pro_Tips.md): This file is a collection of several tips from Terry Hayden.

## IEEE Reference Style

The RPI thesis class defines the layout of the thesis document, except for the references section.
As noted by OGE:

> References to relevant literature should follow the commonly accepted practice in the candidate's field.
> Your advisor will assist you with the proper form of citation.

In all reality, this repository will mostly be used by Computer Science students.
As such, the `IEEE-resources` folder contains the files necessary for an IEEE-styled thesis (originally found [here](http://www.ieee.org/conferences_events/conferences/publishing/templates.html)), including:

- IEEE Style Guide
- IEEE BibTeX resources 
