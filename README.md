# Feature Importance in the Inception (v1) Network

This page shows visualizations of feature importance generated by applying the
technique of **integrated gradients** to the [Inception (v1)][incp-paper]
object recognition network.

In a nutshell, we examine the gradients of certain counterfactual images
obtained by uniformly scaling the pixel intesities in the image at hand, and
aggregate these gradients together. The scaled down images are essentially
points along the straight line path from the actual image to the black image.

A different summarization of the gradients of scaled down images is to directly
visualize them as an animation (GIF), which shows how the gradient of the image
changes as the pixel intensities are scaled up.

The integrated gradients method can be implemented in a few lines of code, 
is applicable to a variety of deep  networks and has some nice mathematical
properties. We recommend reading our [paper][icml-submission], presently under
submission to ICML 2017, for more details.

## Running the code
The code for generating and visualizing integrated gradients is in a single
[Jupyter](http://jupyter.org/) notebook --- [attributions.ipynb][attributions-code].

To run the notebook, please follow the following instructions.
* Clone this repository
  ```
  git clone https://github.com/ankurtaly/Attributions
  ```
* In the same directory, run the Jupyter notebook server.
  ```
  jupyter notebook
  ```
  Instructions for installing Jupyter are available [here](http://jupyter.readthedocs.io/en/latest/install.html).
  Please make sure that you have [TensorFlow][tf], [NumPy][np], and [PIL.Image][pillow] installed for
  Python 2.7.
* Open `attributions.ipynb` and run all cells.

## Visualizations

Below are some visualizations of interior gradients (as a GIF) and integrated
gradients for some images from the ImageNet object recognition dataset. For
comparison, we also show a visualization of the gradients at the actual image.

### Image: 6864d7789068273e
![6864d7789068273e](/Visualizations/IntegratedGradients/6864d7789068273e.jpg)
![6864d7789068273e](/Visualizations/Gifs/6864d7789068273e.gif)
### Image: e60dfdf262c5c74f
![e60dfdf262c5c74f](/Visualizations/IntegratedGradients/e60dfdf262c5c74f.jpg)
![e60dfdf262c5c74f](/Visualizations/Gifs/e60dfdf262c5c74f.gif)
### Image: 35655d94a4557fbb
![35655d94a4557fbb](/Visualizations/IntegratedGradients/35655d94a4557fbb.jpg)
![35655d94a4557fbb](/Visualizations/Gifs/35655d94a4557fbb.gif)
### Image: bda7f59b986d42c0
![bda7f59b986d42c0](/Visualizations/IntegratedGradients/bda7f59b986d42c0.jpg)
![bda7f59b986d42c0](/Visualizations/Gifs/bda7f59b986d42c0.gif)
### Image: 96bb6e948866e5b5
![96bb6e948866e5b5](/Visualizations/IntegratedGradients/96bb6e948866e5b5.jpg)
![96bb6e948866e5b5](/Visualizations/Gifs/96bb6e948866e5b5.gif)
### Image: 80c64f2e27f8784a
![80c64f2e27f8784a](/Visualizations/IntegratedGradients/80c64f2e27f8784a.jpg)
![80c64f2e27f8784a](/Visualizations/Gifs/80c64f2e27f8784a.gif)
### :gImage: b19f875f181025d3
![b19f875f181025d3](/Visualizations/IntegratedGradients/b19f875f181025d3.jpg)
![b19f875f181025d3](/Visualizations/Gifs/b19f875f181025d3.gif)
### Image: 2f401b18be02d7fe
![2f401b18be02d7fe](/Visualizations/IntegratedGradients/2f401b18be02d7fe.jpg)
![2f401b18be02d7fe](/Visualizations/Gifs/2f401b18be02d7fe.gif)
### Image: 92445d6529368418
![92445d6529368418](/Visualizations/IntegratedGradients/92445d6529368418.jpg)
![92445d6529368418](/Visualizations/Gifs/92445d6529368418.gif)
### Image: ba1011c8f9633a49
![ba1011c8f9633a49](/Visualizations/IntegratedGradients/ba1011c8f9633a49.jpg)
![ba1011c8f9633a49](/Visualizations/Gifs/ba1011c8f9633a49.gif)
### Image: 3721d654514bc885
![3721d654514bc885](/Visualizations/IntegratedGradients/3721d654514bc885.jpg)
![3721d654514bc885](/Visualizations/Gifs/3721d654514bc885.gif)
### Image: 12ec21fa7003eae5
![12ec21fa7003eae5](/Visualizations/IntegratedGradients/12ec21fa7003eae5.jpg)
![12ec21fa7003eae5](/Visualizations/Gifs/12ec21fa7003eae5.gif)
### Image: 82262660db12ad85
![82262660db12ad85](/Visualizations/IntegratedGradients/82262660db12ad85.jpg)
![82262660db12ad85](/Visualizations/Gifs/82262660db12ad85.gif)
### Image: b2ab69fbb052b435
![b2ab69fbb052b435](/Visualizations/IntegratedGradients/b2ab69fbb052b435.jpg)
![b2ab69fbb052b435](/Visualizations/Gifs/b2ab69fbb052b435.gif)
### Image: 9a7e268c95022a1c
![9a7e268c95022a1c](/Visualizations/IntegratedGradients/9a7e268c95022a1c.jpg)
![9a7e268c95022a1c](/Visualizations/Gifs/9a7e268c95022a1c.gif)
### Image: 023d8b91c64faf4b
![023d8b91c64faf4b](/Visualizations/IntegratedGradients/023d8b91c64faf4b.jpg)
![023d8b91c64faf4b](/Visualizations/Gifs/023d8b91c64faf4b.gif)
### Image: 7f12674c6943381d
![7f12674c6943381d](/Visualizations/IntegratedGradients/7f12674c6943381d.jpg)
![7f12674c6943381d](/Visualizations/Gifs/7f12674c6943381d.gif)
### Image: 7bcfe0265ad6a2b5
![7bcfe0265ad6a2b5](/Visualizations/IntegratedGradients/7bcfe0265ad6a2b5.jpg)
![7bcfe0265ad6a2b5](/Visualizations/Gifs/7bcfe0265ad6a2b5.gif)
### Image: 518a1c0660c5e32e
![518a1c0660c5e32e](/Visualizations/IntegratedGradients/518a1c0660c5e32e.jpg)
![518a1c0660c5e32e](/Visualizations/Gifs/518a1c0660c5e32e.gif)
### Image: e9c7c07cb5730dac
![e9c7c07cb5730dac](/Visualizations/IntegratedGradients/e9c7c07cb5730dac.jpg)
![e9c7c07cb5730dac](/Visualizations/Gifs/e9c7c07cb5730dac.gif)
<!-- ### Image: 73db3c274688a2e0 -->
<!-- ![73db3c274688a2e0](/Visualizations/IntegratedGradients/73db3c274688a2e0.jpg) -->
<!-- ![73db3c274688a2e0](/Visualizations/Gifs/73db3c274688a2e0.gif) -->
<!-- ### Image: f33412087d9c224e -->
<!-- ![f33412087d9c224e](/Visualizations/IntegratedGradients/f33412087d9c224e.jpg) -->
<!-- ![f33412087d9c224e](/Visualizations/Gifs/f33412087d9c224e.gif) -->
<!-- ### Image: 87fa4cf351b87562 -->
<!-- ![87fa4cf351b87562](/Visualizations/IntegratedGradients/87fa4cf351b87562.jpg) -->
<!-- ![87fa4cf351b87562](/Visualizations/Gifs/87fa4cf351b87562.gif) -->
<!-- ### Image: 69e36e11e9ea9671 -->
<!-- ![69e36e11e9ea9671](/Visualizations/IntegratedGradients/69e36e11e9ea9671.jpg) -->
<!-- ![69e36e11e9ea9671](/Visualizations/Gifs/69e36e11e9ea9671.gif) -->
<!-- ### Image: 870ab22a9f39061d -->
<!-- ![870ab22a9f39061d](/Visualizations/IntegratedGradients/870ab22a9f39061d.jpg) -->
<!-- ![870ab22a9f39061d](/Visualizations/Gifs/870ab22a9f39061d.gif) -->
<!-- ### Image: 700a04c5c2ca6e80 -->
<!-- ![700a04c5c2ca6e80](/Visualizations/IntegratedGradients/700a04c5c2ca6e80.jpg) -->
<!-- ![700a04c5c2ca6e80](/Visualizations/Gifs/700a04c5c2ca6e80.gif) -->
<!-- ### Image: ca29bcc7ead4c115 -->
<!-- ![ca29bcc7ead4c115](/Visualizations/IntegratedGradients/ca29bcc7ead4c115.jpg) -->
<!-- ![ca29bcc7ead4c115](/Visualizations/Gifs/ca29bcc7ead4c115.gif) -->
<!-- ### Image: 1e626579f6ad7b2b -->
<!-- ![1e626579f6ad7b2b](/Visualizations/IntegratedGradients/1e626579f6ad7b2b.jpg) -->
<!-- ![1e626579f6ad7b2b](/Visualizations/Gifs/1e626579f6ad7b2b.gif) -->
<!-- ### Image: 1eb9afc2b4e01ecd -->
<!-- ![1eb9afc2b4e01ecd](/Visualizations/IntegratedGradients/1eb9afc2b4e01ecd.jpg) -->
<!-- ![1eb9afc2b4e01ecd](/Visualizations/Gifs/1eb9afc2b4e01ecd.gif) -->
<!-- ### Image: c27bc2e66f1e66d2 -->
<!-- ![c27bc2e66f1e66d2](/Visualizations/IntegratedGradients/c27bc2e66f1e66d2.jpg) -->
<!-- ![c27bc2e66f1e66d2](/Visualizations/Gifs/c27bc2e66f1e66d2.gif) -->
<!-- ### Image: 5832f36306fb3d66 -->
<!-- ![5832f36306fb3d66](/Visualizations/IntegratedGradients/5832f36306fb3d66.jpg) -->
<!-- ![5832f36306fb3d66](/Visualizations/Gifs/5832f36306fb3d66.gif) -->
<!-- ### Image: 83abcb73307791e8 -->
<!-- ![83abcb73307791e8](/Visualizations/IntegratedGradients/83abcb73307791e8.jpg) -->
<!-- ![83abcb73307791e8](/Visualizations/Gifs/83abcb73307791e8.gif) -->
<!-- ### Image: 82ba0b4b5bb0f7d6 -->
<!-- ![82ba0b4b5bb0f7d6](/Visualizations/IntegratedGradients/82ba0b4b5bb0f7d6.jpg) -->
<!-- ![82ba0b4b5bb0f7d6](/Visualizations/Gifs/82ba0b4b5bb0f7d6.gif) -->
<!-- ### Image: fcd9bbea9f6f5c4a -->
<!-- ![fcd9bbea9f6f5c4a](/Visualizations/IntegratedGradients/fcd9bbea9f6f5c4a.jpg) -->
<!-- ![fcd9bbea9f6f5c4a](/Visualizations/Gifs/fcd9bbea9f6f5c4a.gif) -->
<!-- ### Image: ebc7a444a373cea2 -->
<!-- ![ebc7a444a373cea2](/Visualizations/IntegratedGradients/ebc7a444a373cea2.jpg) -->
<!-- ![ebc7a444a373cea2](/Visualizations/Gifs/ebc7a444a373cea2.gif) -->
<!-- ### Image: 2cc5396cf67cb4ec -->
<!-- ![2cc5396cf67cb4ec](/Visualizations/IntegratedGradients/2cc5396cf67cb4ec.jpg) -->
<!-- ![2cc5396cf67cb4ec](/Visualizations/Gifs/2cc5396cf67cb4ec.gif) -->
<!-- ### Image: f027da6ecb90917c -->
<!-- ![f027da6ecb90917c](/Visualizations/IntegratedGradients/f027da6ecb90917c.jpg) -->
<!-- ![f027da6ecb90917c](/Visualizations/Gifs/f027da6ecb90917c.gif) -->
<!-- ### Image: 093a9eb64c43f424 -->
<!-- ![093a9eb64c43f424](/Visualizations/IntegratedGradients/093a9eb64c43f424.jpg) -->
<!-- ![093a9eb64c43f424](/Visualizations/Gifs/093a9eb64c43f424.gif) -->
<!-- ### Image: 6717aba6a10b230f -->
<!-- ![6717aba6a10b230f](/Visualizations/IntegratedGradients/6717aba6a10b230f.jpg) -->
<!-- ![6717aba6a10b230f](/Visualizations/Gifs/6717aba6a10b230f.gif) -->
<!-- ### Image: 1bd6987fa9219dec -->
<!-- ![1bd6987fa9219dec](/Visualizations/IntegratedGradients/1bd6987fa9219dec.jpg) -->
<!-- ![1bd6987fa9219dec](/Visualizations/Gifs/1bd6987fa9219dec.gif) -->
<!-- ### Image: 15f7f26c4e131021 -->
<!-- ![15f7f26c4e131021](/Visualizations/IntegratedGradients/15f7f26c4e131021.jpg) -->
<!-- ![15f7f26c4e131021](/Visualizations/Gifs/15f7f26c4e131021.gif) -->
<!-- ### Image: 07541d201e18fd86 -->
<!-- ![07541d201e18fd86](/Visualizations/IntegratedGradients/07541d201e18fd86.jpg) -->
<!-- ![07541d201e18fd86](/Visualizations/Gifs/07541d201e18fd86.gif) -->
<!-- ### Image: d113c49533d14d9e -->
<!-- ![d113c49533d14d9e](/Visualizations/IntegratedGradients/d113c49533d14d9e.jpg) -->
<!-- ![d113c49533d14d9e](/Visualizations/Gifs/d113c49533d14d9e.gif) -->
<!-- ### Image: b52346e28fe2f580 -->
<!-- ![b52346e28fe2f580](/Visualizations/IntegratedGradients/b52346e28fe2f580.jpg) -->
<!-- ![b52346e28fe2f580](/Visualizations/Gifs/b52346e28fe2f580.gif) -->
<!-- ### Image: a2c980be2b5d464d -->
<!-- ![a2c980be2b5d464d](/Visualizations/IntegratedGradients/a2c980be2b5d464d.jpg) -->
<!-- ![a2c980be2b5d464d](/Visualizations/Gifs/a2c980be2b5d464d.gif) -->
<!-- ### Image: c55e7d498b6f7786 -->
<!-- ![c55e7d498b6f7786](/Visualizations/IntegratedGradients/c55e7d498b6f7786.jpg) -->
<!-- ![c55e7d498b6f7786](/Visualizations/Gifs/c55e7d498b6f7786.gif) -->
<!-- ### Image: 2587b0bd7d764bd9 -->
<!-- ![2587b0bd7d764bd9](/Visualizations/IntegratedGradients/2587b0bd7d764bd9.jpg) -->
<!-- ![2587b0bd7d764bd9](/Visualizations/Gifs/2587b0bd7d764bd9.gif) -->
<!-- ### Image: c9424338cd2cd36f -->
<!-- ![c9424338cd2cd36f](/Visualizations/IntegratedGradients/c9424338cd2cd36f.jpg) -->
<!-- ![c9424338cd2cd36f](/Visualizations/Gifs/c9424338cd2cd36f.gif) -->
<!-- ### Image: fff0b93993175fb2 -->
<!-- ![fff0b93993175fb2](/Visualizations/IntegratedGradients/fff0b93993175fb2.jpg) -->
<!-- ![fff0b93993175fb2](/Visualizations/Gifs/fff0b93993175fb2.gif) -->
<!-- ### Image: ba024e2cc38f0704 -->
<!-- ![ba024e2cc38f0704](/Visualizations/IntegratedGradients/ba024e2cc38f0704.jpg) -->
<!-- ![ba024e2cc38f0704](/Visualizations/Gifs/ba024e2cc38f0704.gif) -->
<!-- ### Image: c0a9ce885a9c26bc -->
<!-- ![c0a9ce885a9c26bc](/Visualizations/IntegratedGradients/c0a9ce885a9c26bc.jpg) -->
<!-- ![c0a9ce885a9c26bc](/Visualizations/Gifs/c0a9ce885a9c26bc.gif) -->
<!-- ### Image: 70bfca4555cca92e -->
<!-- ![70bfca4555cca92e](/Visualizations/IntegratedGradients/70bfca4555cca92e.jpg) -->
<!-- ![70bfca4555cca92e](/Visualizations/Gifs/70bfca4555cca92e.gif) -->
<!-- ### Image: 8314f5339d6f82ae -->
<!-- ![8314f5339d6f82ae](/Visualizations/IntegratedGradients/8314f5339d6f82ae.jpg) -->
<!-- ![8314f5339d6f82ae](/Visualizations/Gifs/8314f5339d6f82ae.gif) -->
<!-- ### Image: cc61d05004d45a28 -->
<!-- ![cc61d05004d45a28](/Visualizations/IntegratedGradients/cc61d05004d45a28.jpg) -->
<!-- ![cc61d05004d45a28](/Visualizations/Gifs/cc61d05004d45a28.gif) -->
<!-- ### Image: 8577b59a1d19c396 -->
<!-- ![8577b59a1d19c396](/Visualizations/IntegratedGradients/8577b59a1d19c396.jpg) -->
<!-- ![8577b59a1d19c396](/Visualizations/Gifs/8577b59a1d19c396.gif) -->
<!-- ### Image: 4e99de4f5610b052 -->
<!-- ![4e99de4f5610b052](/Visualizations/IntegratedGradients/4e99de4f5610b052.jpg) -->
<!-- ![4e99de4f5610b052](/Visualizations/Gifs/4e99de4f5610b052.gif) -->
<!-- ### Image: 407378360d17f0e6 -->
<!-- ![407378360d17f0e6](/Visualizations/IntegratedGradients/407378360d17f0e6.jpg) -->
<!-- ![407378360d17f0e6](/Visualizations/Gifs/407378360d17f0e6.gif) -->
<!-- ### Image: 7f59ece15328c57d -->
<!-- ![7f59ece15328c57d](/Visualizations/IntegratedGradients/7f59ece15328c57d.jpg) -->
<!-- ![7f59ece15328c57d](/Visualizations/Gifs/7f59ece15328c57d.gif) -->
<!-- ### Image: 8e570672510267d3 -->
<!-- ![8e570672510267d3](/Visualizations/IntegratedGradients/8e570672510267d3.jpg) -->
<!-- ![8e570672510267d3](/Visualizations/Gifs/8e570672510267d3.gif) -->
<!-- ### Image: 17ab5563b441224b -->
<!-- ![17ab5563b441224b](/Visualizations/IntegratedGradients/17ab5563b441224b.jpg) -->
<!-- ![17ab5563b441224b](/Visualizations/Gifs/17ab5563b441224b.gif) -->
<!-- ### Image: d19ebcb973f7904b -->
<!-- ![d19ebcb973f7904b](/Visualizations/IntegratedGradients/d19ebcb973f7904b.jpg) -->
<!-- ![d19ebcb973f7904b](/Visualizations/Gifs/d19ebcb973f7904b.gif) -->
<!-- ### Image: 5cd2c045c7b2b33a -->
<!-- ![5cd2c045c7b2b33a](/Visualizations/IntegratedGradients/5cd2c045c7b2b33a.jpg) -->
<!-- ![5cd2c045c7b2b33a](/Visualizations/Gifs/5cd2c045c7b2b33a.gif) -->

[incp-paper]:http://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Szegedy_Going_Deeper_With_2015_CVPR_paper.pdf
[icml-submission]:http://104.155.136.4:3000/pdf?id=rJzaDdYxx
[attributions-code]:https://github.com/ankurtaly/Attributions/blob/master/attributions.ipynb
[tf]:https://www.tensorflow.org/install/
[np]:https://docs.scipy.org/doc/numpy/user/install.html
[PIL.Image]:http://pillow.readthedocs.io/en/3.1.x/installation.html
