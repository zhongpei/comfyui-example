# comfyui-example

如何使用例子：

* 安装 https://github.com/ltdrdata/ComfyUI-Manager 
* 图片或json文件，拖入浏览器
* 安装缺失的插件
![image](https://github.com/zhongpei/comfyui-example/assets/10387775/20bec2dc-bcc7-4e7b-a68c-868d147814d2)


## 汉化

https://github.com/ZHO-ZHO-ZHO/ComfyUI-ZHO-Chinese.git

## 官方例子

https://comfyanonymous.github.io/ComfyUI_examples/


## 修手
https://github.com/bash-j/mikey_nodes


## 高分辨率

I uploaded these to Git because that's the only place that would save the workflow metadata. I think you have to click the image links. But you can drag and drop these images to see my workflow, which I spent some time on and am proud of.

FYI Comfy's latent handling is SUPERIOR for testing this stuff! Do check it out if you haven't yet.

DreamShaper + SDXL Refiner: https://github.com/jnlarson/jnlarson.github.io/blob/master/Refined.png

Exponential scheduler using DreamShaper model (initial preference): https://github.com/jnlarson/jnlarson.github.io/blob/master/BaseExponential.png

Karras scheduler using DreamShaper model (decent): https://github.com/jnlarson/jnlarson.github.io/blob/master/BaseKarras.png

Simple scheduler using DreamShaper model (too smooth): https://github.com/jnlarson/jnlarson.github.io/blob/master/BaseSimple.png

Normal scheduler using DreamShaper model (too raw): https://github.com/jnlarson/jnlarson.github.io/blob/master/BaseNormal.png

Exponential scheduler with double steps using DreamShaper model (final choice, very nice): https://github.com/jnlarson/jnlarson.github.io/blob/master/BaseExponentialx2.png

Exponential scheduler with double steps using Refiner model (just a test, and too many artifacts): https://github.com/jnlarson/jnlarson.github.io/blob/master/RefinerExponentialx2.png

Conclusion: I could use the same Karras scheduler, but it turns out that Exponential is very accurate to the original.

A little about my step math: Total steps need to be divisible by 5. 4/5 of the total steps are done in the base. Final 1/5 are done in refiner. Testing was done with that 1/5 of total steps being used in the upscaling. Settled on 2/5, or 12 steps of upscaling. Maybe all of this doesn't matter, but I like equations.
