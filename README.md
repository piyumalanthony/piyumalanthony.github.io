## Welcome to My Google Summer of Code 2021 Blog

# GSOC project title - ImageJ: Input/Out Workflows for Active Segmentation Platform

# GSOC project description :

ImageJ is extensively used in major areas of biological and material sciences. Previously developed active segmentation platform as a plugin for ImageJ incorporate Weka 
toolbox-based statistical machine learning algorithms as well as deep learning techniques for trainable image segmentation. The end goal of the active segmentation platform 
for ImageJ is to provide researchers an extensible toolbox enabling them to select custom filters and machine learning algorithms for their research. Especially previously developed semantic segmentation-based techniques are currently in the process of integrating with ImageJ under the Active Segmentation plugin. These techniques are especially based on deep learning algorithms which are state-of-the-art performing procedures for image segmentation.

Under the existing implementation of the active segmentation platform, it only supports users with a limited way to load the ground truth for learning ( at the moment only 
as of the region on interest format (ROI)). Thus, this reduced the usability of the tool and it urges the users to convert the ground truth to the specific format which is designed to be used within the application. Thus this design is not useful for multiple applications. Therefore the main contributions under this project will be to incorporate several ground-truth formats as image-based in which each pixel uniquely belongs to a particular class, partial ground truth format in which instead of the whole image and several partial boxes in an image or stacks are labeled.


<!-- You can use the [editor on GitHub](https://github.com/piyumalanthony/piyumalanthony.github.io/edit/main/README.md) to maintain and preview the content for your website in Markdown files. -->
<!-- 
Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files. -->

<!-- ### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for -->
### Week-1 (2021 June 07 - 2021 June 11)
```markdown
1. What have you been doing this week?

  >>> Testing the existing imageJ plugin for active segmentaions for reported issues.
  >>> TIFF based input/output flow for image and groud-truth loadig implemetation.
  >>> GUI bugs testing and enhancement for input flow of the plugin.
 
2. What are you planning to do next week?
  
  >>> Continue on TIFF based input/output flow implemetaion.
  >>> Testing the implemetation.

3. Is anything blocking your progress?

  >>> There exists few issues regarding dependcy configuraion for the imageJ plugin and the mentors are contated and reported the issue.
```


### Week-2 (2021 June 14 - 2021 June 18)
```markdown
1. What have you been doing this week?

  >>> Fixed issues of project meta information for loading and creating projects for segmentation.
  >>> Fixed issues with Gaussian_K1 filter while loading and applying.
  >>> GUI implemetaion for loading groudtruth from TIFF based groudtruth.
  >>> Fixing issues with testFilter while loading filter.
 
2. What are you planning to do next week?
  
  >>> Pixel based groudtruth loading and dataset creation implemetation.
  >>> Testing the implemetation.

3. Is anything blocking your progress?

  >>> No blockers at the moment.
```


