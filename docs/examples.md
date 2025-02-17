# Demos

## Style Adapter

<p align="center">
  <img src="https://user-images.githubusercontent.com/17445847/222734169-d47789e8-e83c-48c2-80ef-a896c2bafbb0.png" height=450>
</p>

## Color Adapter (Spatial Palette)

<p align="center">
  <img src="https://user-images.githubusercontent.com/17445847/222915829-ccfb0366-13a8-484a-9561-627fabd87d29.png" height=450>
</p>

## Openpose Adapter

<p align="center">
  <img src="https://user-images.githubusercontent.com/17445847/222733916-dc26a66e-d786-4407-8889-b81804862b1a.png" height=450>
</p>

## Canny Adapter (Edge)

<p align="center">
  <img src="https://user-images.githubusercontent.com/17445847/222915813-c8f264bd-1be6-4496-97ff-aec4f6b53788.png" height=450>
</p>

## Multi-adapters
<p align="center">
  <img src="https://user-images.githubusercontent.com/17445847/220939329-379f88b7-444f-4a3a-9de0-8f90605d1d34.png" height=450>
</p>

<div align="center">

*T2I adapters naturally support using multiple adapters together.*

</div><br />
The testing script usage for this example is similar to the command line given below, except that we replaced the pretrained SD model with Anything 4.5 and Kenshi

>python test_composable_adapters.py --prompt "1girl, computer desk, best quality, extremely detailed" --neg_prompt "longbody, lowres, bad anatomy, bad hands, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality" --depth_cond_path examples/depth/desk_depth.png --depth_cond_weight 1.0 --depth_ckpt models/t2iadapter_depth_sd14v1.pth --depth_type_in depth --pose_cond_path examples/keypose/person_keypose.png --pose_cond_weight 1.5 --ckpt models/anything-v4.0-pruned.ckpt --n_sample 4 --max_resolution 524288

[Image source](https://twitter.com/toyxyz3/status/1628375164781211648)
