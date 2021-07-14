![Header](https://github.com/plus-microstate/plus-microstate.github.io/images/header.pdf)

## About +microstate

+microstate is a MATLAB toolbox for performing microstate analysis in sensor- or source-reconstructed EEG or MEG data. +microstate can be used for individual- or group-level analyses, and applied to both resting-state or task-evoked data. As well as microstate analysis, +microstate includes functions for calculating microstate statistics and microstate-segmented functional connectivity, visualisation, and simulation of data. Basic preprocessing is also available in the toolbox, and for more advanced preprocessing +microstate integrates with [Fieldtrip](https://www.fieldtriptoolbox.org), [SPM](https://www.fil.ion.ucl.ac.uk/spm/), [EEGLAB](https://eeglab.org), [LORETA/sLORETA](http://www.uzh.ch/keyinst/loreta), and [Brainstorm](https://neuroimage.usc.edu/brainstorm/). 

## Download and Installation

The easiest way to download the toolbox is to click the following link: 

### [**Download +microstate**](https://github.com/plus-microstate/toolbox/archive/refs/heads/master.zip)

Alternatively, the toolbox can be downloaded from [the toolbox GitHub repository](https://github.com/plus-microstate/toolbox). MATLAB must be installed to run +microstate, which has been tested on MATLAB R2017b and higher. Additionally, the following MATLAB toolboxes are required: [Statistics and Machine Learning](https://www.mathworks.com/products/statistics.html), [Signal Processing](https://www.mathworks.com/products/signal.html), and [Wavelet](https://www.mathworks.com/products/wavelet.html). 

To install the toolbox, unzip the downloaded folder (toolbox-master), then open MATLAB and enter 
```markdown
addpath('PATH/toolbox-master')
```
in the MATLAB console (here `PATH` is the location in which you saved the toolbox-master directory, usually `~/Downloads`). You must either do this each time you open MATLAB, or to permenantly add +microstate to the path you can add toolbox-master to the path using MATLAB's `pathtool` function. 

You can check that the toolbox is properly installed by typing 
```markdown
microstate.functions.toolbox_path
```
in the MATLAB console. If installed correctly, this command returns a string containing the directory with the +microstate toolbox. Otherwise, you will receive an error.

## Citing the toolbox
If you use the +microstate toolbox in your analysis, please cite the toolbox paper (reference given below) and include the URL to the toolbox webpage. 

**Example citation**: 

Microstate segmentation, analysis, and visualisation used the +microstate toolbox for brain microstate analysis in sensor and cortical EEG/MEG (Tait and Zhang (2021); [plus-microstate.github.io](http://plus-microstate.github.io)). 

**Reference**:

Tait and Zhang (2021), _+microstate: A MATLAB toolbox for brain microstate analysis in sensor and cortical EEG/MEG_, Submitted to bioRxiv

## Getting started


## Bug reports and contact
## Publications



You can use the [editor on GitHub](https://github.com/plus-microstate/toolbox_download/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
