# 天空盒

游戏中的天空盒是一个包裹整个场景的立方体，天空盒可以很好的渲染整个环境的气氛，并表达整个场景的环境，。

在 Cocos Creator 3D 中天空盒，如下图所示：
![skybox](skybox/Skybox.jpg)

## 开启天空盒

在 Cocos Creator 3D 中开启天空盒的效果，只需要以下一步：

- Skybox 的面板处于 Scene 节点的属性面板上，将 Enabled 属性勾选上便开启了天空盒
![开启 skybox](skybox/SkyboxPanel.jpg)

## 修改天空盒的环境贴图

在 Cocos Creator 3D 中修改天空盒的环境贴图，是通过设置 TextureCube 类型的资源。
而从资源导入到设置为 TextureCube ，并且设置到 Skybox 中，可以分为以下几步：

1. 导入图片资源。（**注：目前仅支持全景图的分割，暂不支持拼凑散图，请留意更新公告**。）
2. 选中导入的全景图，在右侧的属性面板上，将其设置为 TextureCube 类型，如下图所示。
![设置为 TextureCube](skybox/TextureCube.jpg)
3. 将以上 TextureCube 资源拖入到 Skybox 面板上的 Envmap 属性上。
![设置天空盒的环境贴图](skybox/EnvmapSet.jpg)

完成以上步骤后，就可以在场景中看到最新替换的环境图。

<!-- ## CubeMap

CubeMap 是天空盒的环境贴图资源，在 Cocos Creator 3D 中制作一张 CubeMap ，需要将 6 个面的贴图资源设置到 CubeMap 的相应坐标上。

CubeMap的贴图资源坐标，如下图所示：
![设置为 CubeMap](skybox/CubeMap.jpg) -->

## Skybox 面板

![开启 skybox](skybox/SkyboxDetail.jpg)

以下介绍了面板的所有属性：

属性 | 解释（其它参考盒）
---|---
**enabled** | 是否开启 Skybox
**envmap** | 环境贴图，类型为 TextureCube
**isRGBE** | 环境贴图的像素格式是否为 RGBE
**useIBL** | 是否使用环境光照

<!-- ---

继续前往 [环境光](ambient.md) 说明文档。 -->