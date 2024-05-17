# TitanImage
In this tutorial, we will show how to use the new [Amazon Titan Image Generator](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-image-models.html) on [Amazon Bedrock](https://aws.amazon.com/bedrock/) model to generate (text-to-image) and edit (image-to-image) images.

### Use Cases attempted in this notebook -

1. Text-to-image: Generate coffee machine on the brown wooden table with background of fireplace in modern house.

2. Image-to-image: Add background of ocean with waves crashing in through the window.

3. Image-to-image: Place teddy bear and box of cookies next to the coffee machine

4. Image-to-image: Change color of teddy to brown

 However, there are certain templates that have been known to work.

Broadly, a prompt can be broken down into three pieces:

1. **Type** of image (photograph/sketch/painting/&c.)
2. **Description** of the content (subject/object/environment/scene/&c.), and
3. **Style** of the image (realistic/artistic/&c.).

You can change each of the three parts individually to generate variations of an image. 

Adjectives have been known to play a significant role in the image generation process. 

Also, adding more details help in the generation process.

In order to generate a **realistic** image, you can use phrases such as

```
a photo of
a photograph of
realistic
hyper realistic
```

To generate something more **artistic**, you can use phrases like

```
by Pablo Picasso
oil painting by Rembrandt
landscape art by Frederic Edwin Church
pencil drawing by Albrecht Dürer
```

You can also combine different artists as well.

To generate artistic images by category, you can add the art category in the prompt such as

```
lion on a beach, abstract
```

Some other categories include

```
oil painting
pencil drawing
pop art
digital art
anime
cartoon
futurism
watercolor
manga
&c.
```

You can also include details such as lighting or camera lens such as

```
35mm wide lens
85mm wide lens
```

and details about the framing

```
portrait
landscape
close up
&c.
```

Note that models can generate different images even if same prompt is given multiple times. 

So, you can generate multiple images and select the image that suits your application best.

> ☝️ For more information on Amazon Titan Image Generator prompt engineering, see [Amazon Titan Image Generator Prompt Engineering Best Practices](https://d2eo22ngex1n9g.cloudfront.net/Documentation/User+Guides/Titan/Amazon+Titan+Image+Generator+Prompt+Engineering+Guidelines.pdf). 

