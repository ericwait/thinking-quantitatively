---
title: Understanding Image Analysis for Better Quantitative Experimental Design
author: Eric Wait
date: October 22, 2019
fontfamily: merriweather
fontfamilyoptions: sfdefault
---

## Quotes

> Current limitations in bioimage-informatics techniques are preventing sophisticated optical methods from realiz-ing their full potential...
> The kind of effort required to create a successful bioimage-informatics tool is different from that needed for success in conventional biological research...
> But developing and providing ongoing support for user-friendly tools, although essential for bioimaging, presents challenges to funders and institutions[^unknown2012].

> With sufficient support for bioimage informatics, we expect that the days of manually chosen "representative" images are numbered...
> statistical rigor and clear reporting are critical. In their absence, quantification has limited value, and there is the risk that the mere act of such quantification could lead to false confidence in the results[^unknown2012].


## Questions

1. Battle between complexity and summarization.
2. 

----

## Main Ideas

- State a clear hypothesis or define a model
- Understand the quantification that is needed to support hypothesis or confirm a model
- Design a study that includes quantitative microscopy
- Establish settings and stick to them (homogeneous data collection for nubias and help analysis pipeline)

## Techniques to consider

- Spectral Unmixing
- Deconvolution
- Colocalization
- FRET
- FRAP
- FLIM
- Particle tracking
- Sparse labeling
- Distribution
- Lineaging
- Fission/fusion
- Modeling

## Nuances to be aware of

- Non-linear operations
- Need for fiducial
- Speed of acquisition
- Volume size
- Resolution
- Number of events

-----

- The power of numbers as a summary device
- Automation is key for:
	- High throughput
	- Unbiased / Blind
	- Reproducibility
- Measure features that sand-out during casual observation
	- Know what the eye and brain do to observe features
	- Don't be fooled by what might be filled in as your brain fills in gaps to support a hypothesis
- Planning for analysis during the design phase is key
	- Will what you collect answer/support your questions/hypothesis?
	- Are you going to collect too much or too little data to be practical?
- Collaboration
	- There may be people at your own institution that would love to help
	- There are others that would love to collaborate.

## Pipeline Considerations

### Data cleaning

- What is necessary to get the data into a consistent state for analysis?
	- Details, details, details... key is consistency in naming, collection, and nomenclature
- What is acceptable?
	- I thought I cannot manipulate the data?
- When is it too much or unnecessary?
	- Did I remove what I wanted to measure?
	- Did I create artificial objects that where not in the original?
- Initial bias
	- Have I optimized my datasets or biased my datasets by culling out unexpected or "unrepresentative" data?

### Preprocessing

- Why would I need to processes something before I process it again?
- What techniques are available?
- Why are some operations appropriate in one situations and not in others?
- Could I have collected better data and eliminate preprocessing?
- What versions of the data should I keep?

### Measurements

- What features can I measure?
	- List briefly measurements from the Fiji course.
	- List some more advanced techniques.
	- Encourage thinking outside the box, applying measurements from other fields.
- What features _should_ I measure?
	- Do these measurements answer/support your questions/hypothesis?
	- Are the measurements verifiable?
- Don't use complex measurements when simplistic ones will do.

### Summarization

- What method gets the message across?
	- Graphs / plots
	- Figures
	- Movies
- Ovoid information overload
	- Can the data be presented in more than one way?
	- Can the graphic be split into multiples?

### Reporting

- Methods
	- More is needed
	- Not only sample prep!
- Code
	- Open source
	- State intent of one off or widely applicable
		- It is ok if the intent is that code was intended to be used for a particular study.
		Be upfront.
		Highlight areas of code that are most relevant to help others expand and generalize.
- Conclusions
	- Would other draw the same conclusions after seeing the data?
	- Were the findings significant but not meaningful?
		- For example, two conditions were statistically different, but the differences were below the resolution of the system?

[^unknown2012]: The quest for quantitative microscopy. (2012, July). Nature Methods, 9(7), 627. <https://doi.org/10.1038/nmeth.2102>
[^waters2009]: Waters, J. C. (2009, June 29). Accuracy and precision in quantitative fluorescence microscopy. Journal of Cell Biology, Vol. 185, pp. 1135–1148. <https://doi.org/10.1083/jcb.200903097>
