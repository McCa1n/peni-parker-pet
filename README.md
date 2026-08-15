# Peni Parker 桌宠

这是一个供 ChatGPT/Codex Pets 使用的自定义 Peni Parker 桌宠包。当前形象为潘妮帕克。

## 运行文件

本仓库只有两个运行时必需文件：

| 文件 | 作用 |
| --- | --- |
| `pet.json` | 定义桌宠 ID、显示名称、描述、资源版本和图像路径。 |
| `spritesheet.webp` | Codex 实际加载的动画资源。`pet.json` 中的 `spritesheetPath` 明确指向此文件。 |

请始终将两者放在同一个目录中。运行时不会读取仓库外的预览图、生成脚本或制作过程文件。

## 安装

1. 下载或克隆本仓库。
2. 将整个 `peni-parker` 文件夹复制到 Codex 的桌宠目录：

   ```text
   ~/.codex/pets/peni-parker
   ```

   Windows 常见路径为：

   ```text
   C:\\Users\\<你的用户名>\\.codex\\pets\\peni-parker
   ```

3. 重启 Codex，或刷新桌宠列表。桌宠会以 **Peni Parker** 显示。

## 当前动画资源

`spritesheet.webp` 是当前版本唯一应使用的资源。它采用 Codex Pets v2 格式，图像尺寸为 `1536 x 2288` 像素，并以 `8 x 11` 的帧槽位布局组织；每个槽位为 `192 x 208` 像素。清单中的 `spriteVersionNumber` 为 `2`。

这份 WebP 资源是后续修改后的版本，与早期的像素风预览素材不同。仓库不再保留那张旧预览图，以免将错误的角色风格或帧布局当作当前桌宠内容。

## 修改注意事项

- 不要单独移动或重命名 `spritesheet.webp`，除非同步更新 `pet.json` 中的 `spritesheetPath`。
- 不要改变资源的 `1536 x 2288` 尺寸、`8 x 11` 帧槽位布局或 `192 x 208` 单帧尺寸，否则 Codex 无法按 v2 桌宠规则正确播放。
- 修改桌宠显示名称、说明或 ID 时，请编辑 `pet.json`；修改视觉与动画时，请替换完整的 `spritesheet.webp`，不要混用旧像素风素材。

## 兼容性

该包面向支持 `spriteVersionNumber: 2` 和 WebP 动画资源的 ChatGPT/Codex Pets 环境。

## 说明

这是非官方同人桌宠，与 Marvel、Sony 及 Peni Parker 角色权利方不存在隶属、赞助或授权关系。相关角色名称归其各自权利方所有。
