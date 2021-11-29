# BME 511: Biomedical Signal Processing (Fall 2021)
# Final Project - Report Guidelines

Although the original plan was to have a conference-paper-style report, in order to reduce the time commitment needed to prepare the report, a more "streamlined" format will be used instead. The streamlined format somwhat mirrors the structure used for the project proposal and presentation, but will also allow you to include a more complete and more detailed version of the content. The report should be uploaded as a single PDF file (no ```.ipynb``` files for the report) by **11:59 pm on December 17, 2021**. The report will account for 18% of your final grade, of which 10% is allocated for content (i.e., whether you were able to meet project objectives; and whether you were able to draw reasonable conclusions from your results or the stumbling blocks you may have faced), and 8% is allocated for style (i.e., whether the descriptions are clear, complete, and precise).

In addition to the streamlined report, please provide a copy of your code as **separate** files. These files can be in PDF, ```.ipynb```, ```.py```, or ```.m``` formats.


## Streamlined report format

The report should be formatted to have the following section.

### Title (limit: 20 words) and abstract (limit: 250 words)
This can be the same as what was uploaded with the presentation, or could be an updated version. The abstract should provide a summary of the project.

### Introduction (limit: 500 words)
This is a descriptive text section that provides a concise introdution to the scientific question or engineering problem being addressed, the significance of the problem, and then leads up to a specific objective (or set of objectives). References may be included as necessary. Any domain-specific jargon used in the report should also be defined/introduced here. If it would really help introduce the project, a single figure/illustration may (optionally) be included with this section.

### Methods (limit: 300 words + table)
The methods section should consist of two parts. The first part is a paragraph outlining what data you worked with and what the overall project objectives translate to in the context of this dataset (i.e., the formulation).  This paragraph should be under 300 words and be followed by a table which lists the signal processing steps employed. Optionally, you may include any figures/illustrations and refer to them in the paragraph or table (if that helps understand the methods better). The table should be organized as three columns:

| Description of the signal processing step | Rationale | Inputs and outputs of the step |
|-------------------------------------------|-----------|--------------------------------| 
| | | |

The table can have as many rows as needed to fully describe the steps employed in your project. The description and rationale columns are intended to capture the "what/how" and "why" of each step. They can include information about what each step helps accomplish for the project, how it was carried out, and why that step was appropriate (and/or more appropriate over other possible alternatives if you considered any). The input/output column was added to implicitly encourage your descriptions to be more precise and complete. References (to primary literature, reviews, code documentations etc.) may be included in any column as necessary. Optionally, 3-4 sentences can be added after the table to round out the section (e.g., describe how the steps work together to accomplish the objectives).

### Results (Figures/Tables + "Extended" Captions [under 200 words each])

The results section should simply be a collection of key figures and/or tables of results that help tell the story of your project. Please do **not** include every figure you generate in the process of exploring your data. Only include the ones that are strictly necessary to convey your story. Each figure/table should be accompanied by an "extended" caption that not only describes the components of the plot/table (i.e., what are we looking at), but also describes what the take-home message is from that particular figure/plot in the context of the overall story. **Each "extended" caption should be as brief as possible, but certainly under 200 words**.

With the figures/table included and appropriately captioned, the results section can optionally end with a 3-4 sentence summary of findings. 

> **_NOTE:_**
The "story" being told in the results section doesn't necessarily have to be a story of success. It can also be a story of stumbling blocks faced and the outcomes of what you tried/did in response to those impediments.

### Conclusions (limit: 300 words)

Overall conclusions (regardless of whether you were able to meet project objectives) about the scientific question (or) engineering problem based on your results. Any signal-processing take-aways that you learned through this project may also be included here.

### References (no limit)

Any references cited throughout the report.

### Separate copy of code
No code should be included as part of the streamlined report (which should be in PDF format). Instead, the code used to carry out the project should be provided separately. The separate code files can be in PDF, ```.ipynb```, ```.py```, or ```.m``` format. There is no specific requirement for the organization of the code, and detailed documentation of the code is not necessary. However, comments/headings/spacing should be included to help break up the code into different coherent sections (e.g., different sections for different steps in your methods table). The grading will be based on the report (and not be affected by the organization of the code), but with the caveat that you should submit your code to receive full points for content.

