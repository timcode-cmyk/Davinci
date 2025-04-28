# Fusion 使用指南

本章介绍如何在 Fusion 中使用组、宏和模板，使复杂的效果更有组织、更高效、更易于管理。

---

## 节点组（Groups）

### 什么是节点组？
节点组是节点树中的一种容器，可以容纳多个节点，类似于文件夹容纳多个文件。组可以帮助组织复杂的视觉效果。

- **特点**：
  - 节点数量无限制
  - 支持嵌套子组

### 创建组（Creating Groups）
1. 选择需要分组的节点。
2. 右键单击其中一个节点，选择 **Group**（快捷键：`Command-G`）。
3. 选中的节点会折叠为一个组，显示为单个节点。

### 删除组（Deleting Groups）
1. 选择组节点。
2. 按 `Delete`、`Backspace` 或 `Forward-Delete` 删除组及其包含的所有节点。

### 展开与折叠组（Expanding and Collapsing Groups）
- **展开组**：双击组节点或按 `Command-E`。
- **折叠组**：点击浮动窗口左上角的最小化按钮或再次按 `Command-E`。

### 取消节点组（Ungrouping Nodes）
1. 右键单击组节点。
2. 选择 **Ungroup**，组内的节点会回到主节点树中。

### 保存与重用组（Saving and Reusing Groups）
- **保存组**：右键单击组节点，选择 **Settings > Save As**。
- **加载组**：将保存的组文件拖入节点编辑器。

---

## 宏（Macros）

### 什么是宏？
宏是将一系列节点打包成一个独立的工具，便于重用和共享。

- **优点**：
  - 减少节点树的视觉复杂性
  - 提供自定义用户控件
  - 提高生产效率

### 创建宏（Creating Macros）
1. 选择要包含在宏中的节点。
2. 右键单击，选择 **Macro > Create Macro**。
3. 在宏编辑器中：
   - 输入宏名称。
   - 勾选需要公开的控件。
4. 点击 **Close**，保存宏文件到以下路径：
   - **macOS**: `~/Library/Application Support/Blackmagic Design/DaVinci Resolve/Fusion/Macros/`
   - **Windows**: `C:\Users\username\AppData\Roaming\Blackmagic Design\DaVinci Resolve\Support\Fusion\Macros`
   - **Linux**: `~/.local/share/DaVinciResolve/Fusion/Macros`

### 使用宏（Using Macros）
- 在节点编辑器中右键单击，选择 **Add Tool > Macros**。

### 编辑宏（Re-Editing Macros）
1. 右键单击节点编辑器中的宏。
2. 选择 **Edit Macro**，修改后保存。

---

## 创建 Fusion 模板

Fusion 模板包括标题、过渡、效果和生成器，以下是创建不同模板的步骤。

### 创建标题模板（Creating Title Templates）
1. 创建一个 Fusion 合成，设计标题效果。
2. 右键单击节点，选择 **Macro > Create Macro**。
3. 保存到以下路径：
   - **macOS**: `~/Library/Application Support/Blackmagic Design/DaVinci Resolve/Fusion/Templates/Edit/Titles`
   - **Windows**: `C:\Users\username\AppData\Roaming\Blackmagic Design\DaVinci Resolve\Support\Fusion\Templates\Edit\Titles`
   - **Linux**: `~/.local/share/DaVinciResolve/Fusion/Templates/Edit/Titles`

### 创建过渡模板（Creating Transition Templates）
1. 在 Edit 页面应用过渡效果。
2. 右键单击过渡，选择 **Open in Fusion Page**。
3. 修改节点树后，保存为宏文件到以下路径：
   - **macOS**: `~/Library/Application Support/Blackmagic Design/DaVinci Resolve/Fusion/Templates/Edit/Transitions`
   - **Windows**: `C:\Users\username\AppData\Roaming\Blackmagic Design\DaVinci Resolve\Support\Fusion\Templates\Edit\Transitions`
   - **Linux**: `~/.local/share/DaVinciResolve/Fusion/Templates/Edit/Transitions`

### 创建生成器模板（Creating Generator Templates）
1. 在 Edit 页面拖入 **Fusion Composition**。
2. 打开 Fusion 页面，设计生成器效果。
3. 保存为宏文件到以下路径：
   - **macOS**: `~/Library/Application Support/Blackmagic Design/DaVinci Resolve/Fusion/Templates/Edit/Generators`
   - **Windows**: `C:\Users\username\AppData\Roaming\Blackmagic Design\DaVinci Resolve\Support\Fusion\Templates\Edit\Generators`
   - **Linux**: `~/.local/share/DaVinciResolve/Fusion/Templates/Edit/Generators`

### 创建效果模板（Creating Effect Templates）
1. 在 Fusion 页面设计效果。
2. 保存为宏文件到以下路径：
   - **macOS**: `~/Library/Application Support/Blackmagic Design/DaVinci Resolve/Fusion/Templates/Edit/Effects`
   - **Windows**: `C:\Users\username\AppData\Roaming\Blackmagic Design\DaVinci Resolve\Support\Fusion\Templates\Edit\Effects`
   - **Linux**: `~/.local/share/DaVinciResolve/Fusion/Templates/Edit/Effects`

---

## 模板管理

### 修改模板持续时间
- 使用 **Anim Curves Modifier** 或 **Keyframe Stretcher Modifier** 调整动画时间。

### 创建自定义模板图标
1. 创建一个 PNG 文件（推荐大小：104x58 像素）。
2. 文件名与模板名称相同，扩展名为 `.png`。
3. 将图标文件放在与模板相同的目录中。

### 使用 Fusion 模板包（.drfx）
1. 创建目录结构：Edit/ Effects/ Generators/ Titles/ Transitions/
2. 将模板文件复制到相应目录。
3. 压缩为 `.zip` 文件并重命名为 `.drfx`。
4. 双击 `.drfx` 文件导入 DaVinci Resolve。

---

通过以上步骤，您可以高效地创建、管理和使用 Fusion 的组、宏和模板。

