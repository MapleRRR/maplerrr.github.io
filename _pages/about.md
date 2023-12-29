---
permalink: /
title: "我现在在干啥，我到底能干啥"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!-- What is the matter of the universe made of? Human ask for the answer of all time. I don't know whether it is exists. -->
物质由何组成，人们一直再寻找答案。虽然我不知道这个答案是否存在，但是寻找的过程对于人类（吧，或者对于我？）也充满意义。

高能物理
======
人们探索物质最简单的方法就是拆开看看，现代的拆开“物质”的工具就是加速器。它将物质加速使其相撞，巨大的能量带来了神奇的变化，物质之间遵循着某种规律相互作用并演化，原子核分裂，基本粒子湮灭又产生。撞击的结果能够验证人们天马行空的理论猜测，目前留下的最实用，性价比最高的理论则是标准模型（Standard Model）。2012年，Higgs粒子被发现，标准模型预言的粒子全部被发现，高能物理届欢呼的同时陷入下一个迷茫期（嘎嘎嘎）。

精确计算
======
标准模型已经非常成功的预言了目前所有出现的基本粒子，当然我们知道它还有需要改进的地方。比如无法解释暗物质，中微子质量等等。既然知道有问题还要解决，那我们就力大砖飞来算！给他算的很精确看看实验和计算结果是否有出入。有出入，就有漏洞！那么我们可以抓住漏洞来寻找新物理，这就需要有人想办法怎么算的精确（我就干这事）。

标准模型是基于量子场论所建立的一个非阿贝尔规范理论，在微扰论框架下计算时，费曼图是一个非常方便的工具。但其中会涉及到大量的技术以及难题，如何处理散射振幅、如何处理软共线发散、如何高效完成IBP等，其中有一步是如何计算费曼积分。

![feynman-diagram](/images/The-Feynman-diagrams-for-the-one-particle-irreducible-four-point-function-G-4-p-1-p.png)




Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
