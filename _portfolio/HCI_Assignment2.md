---
title: "Human-Computer Interaction Assignment 2: Accessibility -- Importance of Inclusive Design"
permalink: /portfolio/HCIAccessibility
---

In the past decade, there has been an increased focus of using artificial intelligence to improve accessibility. This focus has lead to amazing assistive technologies such as voice assistance, voice to text, dynamic haptic text displays, and computer vision based guidance devices, just to name a few. With the increasing prevelence of studying human-computer interactions and emphasis on human-centered design processes, the importance of **inclusive design**, in particular with respect to design of accessible technologies, has become a central design principle in approaching ethical development of artificial intelligence. 

## What is Inclusive Design?
<iframe width="560" height="315" src="https://www.youtube.com/embed/-iccWRhKZa8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

While I am still myself working towards better understanding the core principles of the inclusive design processes, the talk above by Kat Holmes provides a great overview. She mentions that the World Health Organization redefined the definition of disability in 2001 to "mismatched interaction between the features of a person's body and the features of the environment in which they live." She discusses how this redefinition solidified in her mind that inclusive user design is centered around identifying mismatches and minimizing ability bias. Ability bias being the tendency to design interfaces that are familiar to your own interactions. I found this to be a profound description of inclusive design and highlights the responsibility of UX and technology designers to conduct a design process that allows them to identify these potential mismatches. 

### Recent Literature  
Recent literature has highlihgted the importance of inclusive and representative design when developing accessible technology. In *Representing Users in Accessibility Research*, Sears and Hanson discuss the use of representative vs. non-representative users during user study design. They argue that only non-representative users and study design that replicates the conditions being evaluated does not capture the interactions those with disabilities have with technologies [1], potentially increasing ability bias. In the article *AI and Accessibility: A discussion of ethical considerations* Dr. Morris, a lead researcher with Microsoft's Ability Research team, highlights the current inclusivity, bias, and privacy limitations of current AI for accessibility research protocols [2] and emphasizes the need for an inclusive design approach that involves representation from a diverse population. Both papers call for design processes that go beyond disability simulations.    

## Example: Image Captioning Assistive Technologies - Increasing Accessibility of Digital Platforms
One example that highlights the importance of inclusive design is in the development of image captioning technologies. A paper presented at the 2020 CHI Conference on Human Factors in Computing systems discussed the image description preferences of visually impared individuals [3] and the limitations of existing image captioning algorithms. While manual methods exist, such as enabling features for content creators to provide alternative text (Instagram example shown in Fig. 1), most digital images do not come with such captions or provided alternative text may be lacking. In the paper, the authors describe how users rely on news article text to cover the content of any images provided and have decreased social media use due to increased reliance on image based platforms. These authors highlight the importance of designing autocaptioning technologies with these demands in mind. However, prior work has found that even technologies that aim to provide this type of captioning for images, fall short of needed performance as they did not undergo inclusive design protocols during development. A paper published in CHI 2013, by Brady, Morris, et al, found that automated captioning algorithms perform poorly on images provided by visually impaired individuals as these algorithms have been trained on images provided by sighted users, which are usually of increased quality in terms of image clarity [4]. The lack of an appropriate dataset has resulted in a non-inclusive design in the development of these algorithms. In an effort to combat these limitations, a VizWiz dataset has been created which contains images along with questions about the image submitted by blind or low vision individuals [5]. This dataset has been used to create algorithms that take into account image quality and diversity of content while developing captioning algorithms [6]. 

<div align="center">
  <img src='/images/hci/instaExample.png'>
</div>
Image Source: https://about.instagram.com/blog/announcements/improved-accessibility-through-alternative-text-support


## Other Interesting Resources for Improving AI Accessibility and Inclusive Design
Below is an interesting talk by Kriti Sharma about human bias in the development of AI technologies: 
<iframe width="560" height="315" src="https://www.youtube.com/embed/BRRNeBKwvNM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Implications for Human-Centered Design
The literature in this area, in particular from the last 2-3 years, has shown an increased focus in design processes that aim to identify mismatches in during prototyping to maximize accessibility of final products. From the published works it is clear that this process must involve 1) increasing participation of represenetative users in the design process, which can come from both improving user recruitment but also by increasing the diversity of product development teams, 2) developing the tools such as datasets to enable development of AI tools, and 3) establishing protocols that minimize bias and increase privacy. 


[1] https://dl.acm.org/doi/pdf/10.1145/1978942.1979268               
[2] https://dl.acm.org/doi/pdf/10.1145/3356727                   
[3] https://dl.acm.org/doi/abs/10.1145/3313831.3376404             
[4] https://www.cs.cmu.edu/~jbigham/pubs/pdfs/2013/visualchallenges.pdf                  
[5] https://vizwiz.org/                 
[6] https://arxiv.org/pdf/2002.08565.pdf                      
