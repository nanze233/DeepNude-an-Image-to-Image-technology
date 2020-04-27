# DeepNude-an-Image-to-Image-technology
GAN evolution graph 2020.

![](paper_images/GAN_2020.png)

This repository contains the pix2pixHD algorithms(proposed by NVIDIA) of [DeepNude](DeepNude_software_itself), and more importantly, the general image generation theory and practice behind DeepNude. This resource includes the TensorFlow2 (Pytorch | PaddlePaddle) implementation of image generation models such as [pix2pix](Pix2Pix), [CycleGAN](CycleGAN), UGATIT, [DCGAN](DCGAN), SinGAN, [VAE](Variational_Autoencoder), ALAE and mGANprior.

这个仓库包含[DeepNude](DeepNude_software_itself)的pix2pixHD(由英伟达提出)算法，更重要的是DeepNude背后通用的图像生成理论与实践研究。本资源包含[pix2pix](Pix2Pix), [CycleGAN](CycleGAN), UGATIT, [DCGAN](DCGAN), SinGAN, [VAE](Variational_Autoencoder), ALAE and mGANprior 等图像生成模型的 [TensorFlow2](https://www.tensorflow.org/) (Pytorch | PaddlePaddle) 实现。

---

## Content of this resource 本资源内容

|English|中文|
|-|-|
|What is DeepNude?|什么是 DeepNude?|
|Fake Image Generation and Image-to-Image Demo |试玩Demo|
|DeepNude Algorithm: Normal to Pornography Image|由正常图像生成色情图像|
|NSFW: Pornography to Normal Image, Pornographic Image Detection|由色情图像生成正常图像，色情图像检测|
|GAN Image Generation Theoretical Research|  GAN 图像生成理论研究|
|GAN Image Generation Practice Research|  GAN 图像生成实践研究|
|DeepNude to DeepFakes|DeepNude 进阶 DeepFakes|
|Future|					                     展望未来|

---

## What is DeepNude? 什么是 DeepNude?
DeepNude uses a slightly modified version of the [pix2pixHD](https://github.com/NVIDIA/pix2pixHD) GAN architecture, quoted from deepnude_official. pix2pixHD is a general-purpose Image2Image technology proposed by NVIDIA. Obviously, DeepNude is the wrong application of artificial intelligence technology, but it uses Image2Image technology for researchers and developers working in other fields such as fashion, film and visual effects.

[DeepNude](https://github.com/yuanxiaosc/DeepNude-an-Image-to-Image-technology/tree/master/DeepNude_software_itself)使用了一个稍微修改过的 [pix2pixHD](https://github.com/NVIDIA/pix2pixHD) GAN 架构。pix2pixHD是由NVIDIA提出的一种通用的Image2Image技术。显然，DeepNude是人工智能技术的错误应用，但它使用的Image2Image技术对于在时尚，电影和视觉效果等其他领域工作的研究人员和开发人员非常有用。

---

## Fake Image Generation Demo

This section provides a fake image generation demo that you can use as you wish. They are fake images generated by StyleGAN without any copyright issues. Note: Each time you refresh the page, a new fake image will be generated, pay attention to save!

这部分提供一个试玩的假图片生成Demo，你可以随心所欲的使用它们。它们是由StyleGAN生成的假图片，没有任何版权问题。每次刷新网页都会生成新的假图像，注意保存！

+ [Click to generate fake person image 点击生成假人图像](https://thispersondoesnotexist.com/)
+ [Click to generate fake cat image 点击生成假猫图像](http://thesecatsdonotexist.com/)
+ [Click to generate fake waifu image 点击生成假老婆图像](https://www.thiswaifudoesnotexist.net/)


## Image-to-Image Demo

This section provides a demo of Image-to-Image Demo: Black and white stick figures to colorful cats, shoes, handbags. DeepNude software mainly uses Image-to-Image technology, which theoretically converts the images you enter into any image you want. You can experience Image-to-Image technology in your browser by clicking Image-to-Image Demo below.

这一部分提供一个试玩的 Image-to-Image Demo：黑白简笔画到色彩丰富的猫、鞋、手袋。DeepNude 软件主要使用了Image-to-Image技术，该技术理论上可以把你输入的图片转换成任何你想要的图片。你可以点击下方的Image-to-Image Demo在浏览器中体验Image-to-Image技术。

[Try Image-to-Image Demo](https://affinelayer.com/pixsrv/)

An example of using this demo is as follows：

![](paper_images/2017_Phillip_pix2pix_examples_edges2cats.png)

In the left side box, draw a cat as you imagine, and then click the process button, you can output a model generated cat.

在左侧框中按照自己想象画一个简笔画的猫，再点击process按钮，就能输出一个模型生成的猫。

---

## :underage: DeepNude Algorithm
> DeepNude is a pornographic software that is forbidden by minors. If you are not interested in DeepNude itself, you can skip this section and see the general Image-to-Image theory and practice in the following chapters. DeepNude 是一款含有色情的软件，未成年人禁止使用。如果你对DeepNude本身不感兴趣，可以直接跳过本节，查看后面章节中通用的Image-to-Image理论与实践研究。

[DeepNude_software_itself](DeepNude_software_itself) content:
1. Official DeepNude Algorithm(Based on Pytorch)
2. DeepNude software usage process and evaluation of advantages and disadvantages.



### :+1: NSFW
> Recognition and conversion of five types of images [porn, hentai, sexy, natural, drawings]. Correct application of image-to-image technology.

NSFW(Not Safe/Suitable For Work) is a large-scale image dataset containing five categories of images [porn, hentai, sexy, natural, drawings]. Here, CycleGAN is used to convert different types of images, such as porn->natural.

使用CycleGAN神经网络模型实现 [porn, hentai, sexy, natural, drawings] 这些类别图像的转换，比如色情图像到安全/中性的图像转换。

1. [Click to try pornographic image detection Demo 点击尝试色情图片检测](https://nsfwjs.com/)
2. [Click Start NSFW Research](NSFW)

---

## Image Generation Theoretical Research

This section describes DeepNude-related AI/Deep Learning theory (especially computer vision) research. If you like to read the paper and use the latest papers, enjoy it.

这一部分阐述DeepNude相关的人工智能/深度学习理论（特别是计算机视觉）研究，如果你喜欢阅读论文使用最新论文成果，尽情享用吧。

[Click here to systematically understand GAN](GAN_History)

[Click here to systematically image-to-image-papers](https://github.com/lzhbrian/image-to-image-papers/blob/master/README.md)

### 1. Pix2Pix

+ 论文 Berkeley 2017 paper [Image-to-Image Translation with Conditional Adversarial Networks](https://arxiv.org/abs/1611.07004)
+ 主页 [Pix2Pix homepage](https://phillipi.github.io/pix2pix/)
+ 代码 code [pix2pix](https://github.com/phillipi/pix2pix)
+ Run in Google Colab [pix2pix.ipynb](https://github.com/tensorflow/docs/blob/master/site/en/r2/tutorials/generative/pix2pix.ipynb)

**效果**

![](paper_images/2017_Phillip_pix2pix_examples.jpg)

[Image-to-Image Translation with Conditional Adversarial Networks](https://arxiv.org/abs/1611.07004) is a general solution for the use of conditional confrontation networks as an image-to-image conversion problem proposed by the University of Berkeley.

[Image-to-Image Translation with Conditional Adversarial Networks](https://arxiv.org/abs/1611.07004) 是伯克利大学研究提出的使用条件对抗网络作为图像到图像转换问题的通用解决方案。

### 2. Pix2PixHD
> DeepNude mainly uses this Image-to-Image(Pix2PixHD) technology.

+ 论文 NVIDIA 2018 [High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs](https://arxiv.org/abs/1711.11585)
+ 主页 [Pix2PixHD homepage](https://tcwang0509.github.io/pix2pixHD/)
+ 代码 code [pix2pixHD](https://github.com/NVIDIA/pix2pixHD)

**效果**

![](paper_images/2018_NVIDIA_Pix2PixHD_example.png)
![](paper_images/2018_NVIDIA_Pix2PixHD_example_2.png)

Get high resolution images from the semantic map. The semantic graph is a color picture. The different color blocks on the map represent different kinds of objects, such as pedestrians, cars, traffic signs, buildings, and so on. Pix2PixHD takes a semantic map as input and produces a high-resolution, realistic image. Most of the previous techniques can only produce rough, low-resolution images that don't look real. This research has produced images with a resolution of 2k by 1k, which is very close to full HD photos.

从语义图上获得高分辨率图片。语义图是一幅彩色图片，图上的不同色块代表不同种类物体，如行人、汽车、交通标志、建筑物等。Pix2PixHD将一张语义图作为输入，并由此生成了一张高分辨率的逼真的图像。之前的技术多数只能生成粗糙的低分辨率的图片，看起来也不真实。而这个研究却生成了2k乘1k分辨率的图像，已经很接近全高清的照片。

### 3. CycleGAN

+ 论文 Berkeley 2017 paper [Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks](https://arxiv.org/abs/1703.10593)
+ 主页 [CycleGAN homepage](https://junyanz.github.io/CycleGAN/)
+ 代码 code [CycleGAN](https://github.com/junyanz/CycleGAN)
+ Run in Google Colab [cyclegan.ipynb](https://github.com/tensorflow/docs/blob/master/site/en/r2/tutorials/generative/cyclegan.ipynb)

**效果**

![](paper_images/2017_Zhu_CycleGAN_examples.jpg)

CycleGAN uses a cycle consistency loss to enable training without the need for paired data. In other words, it can translate from one domain to another without a one-to-one mapping between the source and target domain. This opens up the possibility to do a lot of interesting tasks like photo-enhancement, image colorization, style transfer, etc. All you need is the source and the target dataset.

CycleGAN使用循环一致性损失函数来实现训练，而无需配对数据。换句话说，它可以从一个域转换到另一个域，而无需在源域和目标域之间进行一对一映射。这开启了执行许多有趣任务的可能性，例如照片增强，图像着色，样式传输等。您只需要源和目标数据集。

### 4. UGATIT

+ 论文 NCSOFT 2019 paper [Unsupervised Generative Attentional Networks with Adaptive Layer-Instance Normalization for Image-to-Image Translation](https://github.com/taki0112/UGATIT)
+ 代码 code [UGATIT-TensorFlow](https://github.com/taki0112/UGATIT)  | [UGATIT-Pytorch](https://github.com/znxlwm/UGATIT-pytorch)
+ [UGATIT 原理解析](https://zhuanlan.zhihu.com/p/76936166)
+ [UGATIT 实验复现](https://zhuanlan.zhihu.com/p/76979105)

**效果**

![](paper_images/2019_NCSOFT_UGATIT_example.jpg)

UGATIT is a novel method for unsupervised image-to-image translation, which incorporates a new attention module and a new learnable normalization function in an end-to-end manner. UGATIT can do both image conversions that require Holistic Changes, and image conversions that require Large Shape Changes. It can be seen as an enhanced version of CycleGAN, a more efficient general image conversion framework.

UGATIT是一种新的无监督图像到图像转换方法，它以端到端的方式结合了新的注意模块和新的可学习的归一化功能。UGATIT既可以做需要整体变化 (Holistic Changes) 的图片转换，也可以做需要大幅形状变化 (Large Shape Changes ) 的图片转换。它可以看做CycleGAN的加强版本，是一种效果更好的通用图片转换框架。

### 5. StyleGAN

+ 论文 NVIDIA 2018 paper [A Style-Based Generator Architecture for Generative Adversarial Networks](https://arxiv.org/abs/1812.04948)
+ 代码 code [stylegan](https://github.com/NVlabs/stylegan)

**效果**

![](paper_images/2019_NVIDIA_StyleGAN_example.png)

Source A + Source B (Style) = ?

StyleGAN can not only generate fake images source A and source B, but also combine the content of source A and source B from different strengths, as shown in the following table.

StyleGAN 不仅可以生成假的图片source A 和 source B，还可以结合从不同的力度上结合source A的内容和 source B的样式，具体说明如下表。

|Style 等级（源自 Source B）|Source A|Source B|
|-|-|-|
|高等级（粗略）|所有颜色（眼睛，头发，光线）和细节面部特征来自Source A|继承Source B高级的面部特征，如姿势、一般的发型、脸部形状和眼镜|
|中等级|姿势、一般的面部形状和眼镜来自Source A|继承Source B中级的面部特征 ，如发型，张开/闭着的眼睛|
|高等级（细微）|主要面部内容来自Source A|继承Source B高级面部特征，如颜色方案和微观结构|

#### StyleGAN2
Without increasing the amount of calculation of StyleGAN, while solving the image artifacts generated by StyleGAN and obtaining high-quality images with better details, StyleGAN2 implements a new SOTA for unconditional image modeling tasks.

+ 论文 NVIDIA 2019 paper [Analyzing and Improving the Image Quality of StyleGAN](https://arxiv.org/abs/1912.04958)
+ 代码 code [stylegan2](https://github.com/NVlabs/stylegan2)
+ Run in Google Colab [stylegan2](https://colab.research.google.com/drive/1ShgW6wohEFQtqs_znMna3dzrcVoABKIH)

在不增加StyleGAN计算量的条件下，在解决了StyleGAN生成图像伪影的同时还能得到细节更好的高质量图像，StyleGAN2实现了无条件图像建模任务上新的 SOTA。

### 6. Image Inpainting 图像修复

+ 论文 NVIDIA 2018 paper [Image Inpainting for Irregular Holes Using Partial Convolutions](https://arxiv.org/abs/1804.07723) and [Partial Convolution based Padding](https://arxiv.org/abs/1811.11718).
+ 代码 Paper code [partialconv](https://github.com/NVIDIA/partialconv)。

**效果**

![](paper_images/2018_NVIDIA_Image_Inpainting_examples.png)

In the image interface of [Image_Inpainting(NVIDIA_2018).mp4](https://github.com/yuanxiaosc/DeepNude-an-Image-to-Image-technology/raw/master/paper_images/Image_Inpainting(NVIDIA_2018).mp4) video, you only need to use tools to simply smear the unwanted content in the image. Even if the shape is very irregular, NVIDIA's model can “restore” the image with very realistic The picture fills the smeared blank. It can be described as a one-click P picture, and "no ps traces." The study was based on a team from Nvidia's Guilin Liu et al. who published a deep learning method that could edit images or reconstruct corrupted images, even if the images were worn or lost pixels. This is the current 2018 state-of-the-art approach.

在 [Image_Inpainting(NVIDIA_2018).mp4](https://github.com/yuanxiaosc/DeepNude-an-Image-to-Image-technology/raw/master/paper_images/Image_Inpainting(NVIDIA_2018).mp4) 视频中左侧的操作界面，只需用工具将图像中不需要的内容简单涂抹掉，哪怕形状很不规则，NVIDIA的模型能够将图像“复原”，用非常逼真的画面填补被涂抹的空白。可谓是一键P图，而且“毫无ps痕迹”。该研究来自Nvidia的Guilin Liu等人的团队，他们发布了一种可以编辑图像或重建已损坏图像的深度学习方法，即使图像穿了个洞或丢失了像素。这是2018 state-of-the-art的方法。

### 7. SinGAN
ICCV2019 Best paper - Marr prize

+ 论文 Israel Institute of Technology 2019 paper [SinGAN: Learning a Generative Model from a Single Natural Image](https://arxiv.org/abs/1905.01164)
+ 主页 [SinGAN homepage](http://webee.technion.ac.il/people/tomermic/SinGAN/SinGAN.htm)
+ 代码 code [SinGAN-Pytorch](https://github.com/tamarott/SinGAN)
+ 视频展示 Video Show [SinGAN for single image animation](https://youtu.be/xk8bWLZk4DU)
+ [SinGAN 原理解析](https://www.jiqizhixin.com/articles/2019-10-29-2)

**效果**

![](paper_images/2019_Tamar_SinGAN_example.png)
We introduce SinGAN, an unconditional generative model that can be learned from a single natural image. Our model is trained to capture the internal distribution of patches within the image, and is then able to generate high quality, diverse samples that carry the same visual content as the image. SinGAN contains a pyramid of fully convolutional GANs, each responsible for learning the patch distribution at a different scale of the image. This allows generating new samples of arbitrary size and aspect ratio, that have significant variability, yet maintain both the global structure and the fine textures of the training image. In contrast to previous single image GAN schemes, our approach is not limited to texture images, and is not conditional (i.e. it generates samples from noise). User studies confirm that the generated samples are commonly confused to be real images. We illustrate the utility of SinGAN in a wide range of image manipulation tasks.

在这篇论文中，研究者介绍了一种无监督的生成模型 SinGAN，它以一种无条件约束的方式从单张自然图像中学习知识。经过训练，研究者的模型能捕捉图像块（patch）的内部分布，从而生成高质量、多样化的样本，并承载与训练图像相同的视觉内容。

SinGAN 包含一个全卷积金字塔 GAN，金字塔的每一层负责学习不同比例的图像块分布。这样就能生成具有任意大小和横纵比的新样本，这种生成样本明显具有可变性，但同时又能保持真实图像的全局结构与精细纹理。与之前的单图像 GAN 相比，研究者的方法不仅能生成纹理图像，同时它还以一种无条件约束的方式生成。SinGAN 通过使用多尺度对抗训练方案，从多种尺度学习了图像块信息。这样一来，模型就可以生成新的真实图像样本，其中在创建新的目标属性和结构的同时还保留了原始的图像块分布信息。如上展示了不同尺度图像的生成效果。研究者在最后还表明，SinGAN 生成的图像经常被人类弄混，它们与真实图像没什么差别。

### 8. ALAE

+ 论文 2020 paper [Adversarial Latent Autoencoders](https://arxiv.org/abs/2004.04467)
+ 代码 code [ALAE](https://github.com/podgorskiy/ALAE)

**效果**

![](https://user-images.githubusercontent.com/3229783/79670218-63080d80-818f-11ea-9e50-927b8af3e7b5.gif)

Although studied extensively, the issues of whether they have the same generative power of GANs, or learn disentangled representations, have not been fully addressed. We introduce an autoencoder that tackles these issues jointly, which we call Adversarial Latent Autoencoder (ALAE). It is a general architecture that can leverage recent improvements on GAN training procedures.

关于自编码器有两个疑问尚未得到解决：自编码器是否具备和 GAN 同等的生成能力？自编码器能否学习解耦表征？美国西弗吉尼亚大学的研究者提出一种新型自编码器 Adversarial Latent Autoencoder (ALAE)，试图解决以上问题。ALAE是一个通用架构，它能够利用近期GAN在训练方面的改进。研究者表示ALAE具备与GAN相当的生成能力，且能够学习解耦表征。

### 9. mGANprior

+ 论文 2020 paper [Image Processing Using Multi-Code GAN Prior](https://arxiv.org/abs/1912.07116)
+ 主页 [mGANprior homepage](https://genforce.github.io/mganprior/)
+ 代码 code [mganprior](https://github.com/genforce/mganprior)

**效果**

![](paper_images/2020_Gujinjin_mGANprior_example.jpg)

Despite the success of Generative Adversarial Networks (GANs) in image synthesis, applying trained GAN models to real image processing remains challenging. Previous methods typically invert a target image back to the latent space either by back-propagation or by learning an additional encoder. However, the reconstructions from both of the methods are far from ideal. In this work, we propose a novel approach, called mGANprior, to incorporate the well-trained GANs as effective prior to a variety of image processing tasks.

为了让训练好的GAN能用于处理图像，现有方法尝试以重新反向传播（寻找合适的Z）或者添加一个额外的编码器encoder将图像映射到潜在空间。但多数情况下两者的重建并不理想。在这项工作中提出一种新的逆映射（image->Z）方法，将训练好的GAN作为一个有效的先验去处理多种图像处理任务。

---

## Image Generation Practice Research
> These models are based on the latest implementation of TensorFlow2.

This section explains DeepNude-related AI/Deep Learning (especially computer vision) code practices, and if you like to experiment, enjoy them.

这一部分阐述DeepNude相关的人工智能/深度学习（特别是计算机视觉）代码实践，如果你喜欢动手做实验，尽情享用它们。

### 1. Pix2Pix

Use the Pix2Pix model (Conditional Adversarial Networks) to implement black and white stick figures to color graphics, flat houses to stereoscopic houses and aerial maps to maps.

使用Pix2Pix模型（Conditional Adversarial Networks）实现黑白简笔画到彩图、平面房屋到立体房屋和航拍图到地图等功能。

[Click Start Experience 1](Pix2Pix)

### 2. Pix2PixHD

Under development... First you can use the [official implementation](https://github.com/NVIDIA/pix2pixHD)

### 3. CycleGAN

The CycleGAN neural network model is used to realize the four functions of photo style conversion, photo effect enhancement, landscape season change, and object conversion.

使用CycleGAN神经网络模型实现照片风格转换、照片效果增强、照片中风景季节变换、物体转换四大功能。

[Click Start Experience 3](CycleGAN)

### 4. DCGAN

DCGAN is used to achieve random number to image generation tasks, such as face generation. 使用DCGAN来实现随机数到图片生成任务，比如人脸生成。

[Click Start Experience 4](DCGAN)

### 5. Variational Autoencoder (VAE)
VAE is used to achieve random number to image generation tasks, such as face generation. 使用VAE来实现随机数到图片生成任务，比如人脸生成。

[Click Start Experience 5](Variational_Autoencoder)

### 6. Neural style transfer
Use VGG19 to achieve image style migration effects, such as photo changes to oil paintings and comics. 使用VGG19来实现图片风格迁移效果，比如照片变油画、漫画。

[Click Start Experience 6](Neural_style_transfer)

..........................................................................

如果你是使用[PaddlePaddle](https://github.com/PaddlePaddle/Paddle)的用户，可以参考以上模型的Paddle版本 [图像生成模型库 PaddleGAN](https://github.com/PaddlePaddle/models/tree/develop/PaddleCV/PaddleGAN)。

---

## DeepFakes (Promotion of DeepNude)
> DeepFakes can be seen as an upgraded version of DeepNude, which uses a deep learning model to generate a series of techniques that can be faked, such as fake images, fake audio, and fake videos. DeepFakes可以看做是DeepNude的升级版，它包含使用深度学习模型生成一系列可以以假乱真的东西技术，例如假的图像、假的音频和假的视频。

### Realistic Speech-Driven Facial Animation with GANs
One photo + One audio = Composite Video

We propose a temporal GAN capable of producing animated faces using only a still image of a person and an audio clip containing speech. The videos generated using this model do not only produce lip movements that are synchronized with the audio but also exhibit characteristic facial expressions such as blinks, brow raises etc. This extends our previous model by separately dealing with audio-visual synchronization and expression generation. Our improved model works on "in-the-wild" unseen faces and is capable of capturing the emotion of the speaker and reflecting it in the facial expression.

一张照片 + 一段音频 = 合成视频

我们提出了一种 temporal GAN，其能够仅使用人的静止图像和包含语音的音频剪辑来产生动画面部。 使用此模型生成的视频不仅可以产生与音频同步的唇部动作，还可以呈现特有的面部表情，例如眨眼，眉毛等，同时能够捕捉说话者的情绪并将其反映在面部表情中。

+ 论文 Samsung and Imperial College London 2019 paper [Realistic Speech-Driven Facial Animation with GANs](https://arxiv.org/abs/1906.06337)
+ 主页 [Facial Animation homepage](https://sites.google.com/view/facial-animation)
+ 代码 code [Speech-Driven Animation](https://github.com/DinoMan/speech-driven-animation)
+ [中文版论文浅析](https://www.infoq.cn/article/CM72xuNm35pNdrw7p_yT?utm_source=related_read&utm_medium=article) [English version paper analysis](https://www.theverge.com/2019/6/20/18692671/deepfake-technology-singing-talking-video-portrait-from-a-single-image-imperial-college-samsung)


**Interested in DeepFakes?**

[Click to start systematic learning DeepFakes](DeepFakes)

---

## Future

[Click read more...](Future)
