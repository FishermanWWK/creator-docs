---
title: Model tab
description: The Model tab contains tools for manipulating 3D objects and models, working with physical constraints, and more.
---

import BetaAlert from '../includes/beta-features/beta-alert.md'

The **Model** tab contains tools for manipulating 3D objects in the workspace, creating detailed models, working with physical constraints, and adding advanced objects.

<img src="../assets/studio/general/Toolbar-Model-Tab.png" width="830" alt="Model tab indicated in Studio toolbar" />

## Transform tools

The primary transform tools include **Select**, **Move**, **Scale**, **Rotate**, and **Transform**. When you choose a tool, visual draggers display on the selected object in the 3D viewport.

<img src="../assets/studio/general/Model-Tab-Transform-Tools.png"
   width="830" alt="Transform tools indicated in Model tab" />

<GridContainer numColumns="3">
  <figure>
    <img src="../assets/modeling/parts/Transform-Move-SM.png" alt="Move draggers shown on part in 3D viewport" />
    <figcaption>Move</figcaption>
  </figure>
  <figure>
    <img src="../assets/modeling/parts/Transform-Scale-SM.png" alt="Scale draggers shown on part in 3D viewport" />
    <figcaption>Scale</figcaption>
  </figure>
  <figure>
    <img src="../assets/modeling/parts/Transform-Rotate-SM.png" alt="Rotate draggers shown on part in 3D viewport" />
    <figcaption>Rotate</figcaption>
  </figure>
</GridContainer>

Tool transform **snapping increments** are based on **studs** for moving/scaling or **degrees** for rotating, each adjustable. While transforming, you can temporarily toggle snapping by holding the <kbd>Shift</kbd> key.

<Alert severity="info">
If the selected object and its visual draggers are not currently in view within the 3D viewport, you can press the <kbd>Tab</kbd> key to "summon" the draggers to your mouse pointer position, allowing you to transform the selected object from your current viewpoint.
</Alert>

### Mode

The **Mode** selector toggles between standard geometric transformations and [simulation of mechanical constraints](../physics/mechanical-constraints.md#simulate-constraints) while moving or rotating parts.

<img src="../assets/studio/general/Model-Tab-Mode.png" width="768" alt="Mode selector indicated in Model tab" />

### Collisions

The **Collisions** checkbox toggles the collisions state when you're transforming objects. If collisions are **off**, you can move, scale, and rotate objects so that they overlap each other; if collisions are **on**, you cannot transform objects to overlap other objects.

<img src="../assets/studio/general/Model-Tab-Collisions-On.png"
   width="768" alt="Collisions checkbox indicated in Model tab" />

### Transform snapping

Snap increments for tool transforms are based on **studs** for moving/scaling or **degrees** for rotating. To enable or disable snapping:

- Temporarily toggle snapping either on or off by holding <kbd>Shift</kbd> while transforming.
- Toggle the checkbox next to **Rotate** or **Move**, and adjust the rotation/transform increments via the input fields.

  <img src="../assets/studio/general/Model-Tab-Transform-Snapping.png" width="768" alt="Transform snapping tools indicated in Model tab" />

### Transform coordinates

<kbd>Ctrl</kbd><kbd>L</kbd> on Windows or <kbd>⌘</kbd><kbd>L</kbd> on Mac toggles between transforming an object relative to **world** coordinates or the object's **local** coordinates. When in local mode, an **L** symbol appears to the lower-right of the object.

<Tabs>
  <TabItem label="World">
    <img src="../assets/modeling/parts/Move-World-Orientation.png" width="720" height="405" alt="Part draggers in World orientation mode" />
  </TabItem>
  <TabItem label="Local">
    <img src="../assets/modeling/parts/Move-Local-Orientation.png" width="720" height="405" alt="Part draggers in Local orientation mode" />
  </TabItem>
</Tabs>

## Pivot tools

The **Pivot** tools give you full control over the points around which objects rotate and translate. See [Pivot&nbsp;Tools](../studio/pivot-tools.md) for details.

<img src="../assets/studio/general/Model-Tab-Pivot-Tools.png" width="768" alt="Pivot Tools indicated in Model tab" />

## Align Tool

The **Align Tool** button opens a set of tools for aligning objects or groups of objects along the X, Y, or Z axes. For more information, see [Align&nbsp;Tool](../studio/align-tool.md).

<img src="../assets/studio/general/Model-Tab-Align-Tool.png" width="660" alt="Align Tool indicated in Model tab" />

## Part insertion

The **Part** button inserts a new part into the workspace. Clicking the small dropdown arrow on the button lets you select either **Block**, **Sphere**, **Wedge**, **Corner&nbsp;Wedge**, or **Cylinder**. For more information, see [Parts](../parts/index.md).

<img src="../assets/studio/general/Model-Tab-Part-Tools.png" width="660" alt="Part menu indicated in Model tab" />

## Color widget

Clicking the small dropdown arrow on the **Color** widget reveals a hexagonal color picker.

<img src="../assets/studio/general/Model-Tab-Color-Picker.png" width="704" alt="Studio's Model tab with the Color widget's hexagonal picker." />

By default, clicking the overall **Color** button applies the chosen color to any **selected** parts. If you prefer a fill/paint workflow instead, toggle on **Color&nbsp;Action&nbsp;as&nbsp;Tool** and then click parts in the 3D viewport to apply the chosen color.

<img src="../assets/studio/general/Model-Tab-Color-Action-As-Tool.png" width="704" alt="Studio's Model tab with the Color Action as Tool selector indicated." />

<Alert severity="success">
For alternative ways to apply custom colors, see [Coloring Parts](../parts/index.md#colors-popup).
</Alert>

## Material widget

Clicking the small dropdown arrow on the **Material** widget reveals a [material](../parts/materials.md) picker.

<img src="../assets/studio/general/Model-Tab-Material-Picker.png" width="704" alt="Studio's Model tab with the Material widget's picker." />

By default, clicking the overall **Material** button applies the chosen material to any **selected** parts. If you prefer a fill/paint workflow instead, toggle on **Material&nbsp;Action&nbsp;as&nbsp;Tool** and then click parts in the 3D viewport to apply the chosen material.

<img src="../assets/studio/general/Model-Tab-Material-Action-As-Tool.png" width="704" alt="Studio's Model tab with the Material Action as Tool selector indicated." />

## Texture Generator

<BetaAlert betaName="Texture Generator" leadIn="This tool is currently in beta. Enable it through " leadOut="." components={props.components} />

The [Texture Generator](../studio/texture-generator.md) tool quickly creates custom textures for meshes through text prompts.

<img src="../assets/studio/general/Model-Tab-Texture-Generator.png" width="704" alt="Texture Generator indicated in Model tab" />

## Group tools

You can group objects into a [model](../parts/models.md) by selecting them and clicking the **Group** button. This action has a default shortcut of <kbd>Ctrl</kbd><kbd>G</kbd> (Windows) or <kbd>⌘</kbd><kbd>G</kbd> (Mac).

Alternatively, you can group objects into a [folder](../studio/explorer.md#organize-by-folders) by clicking the small arrow next to the button and selecting **Group as a Folder**. This action has a default shortcut of <kbd>Alt</kbd><kbd>Ctrl</kbd><kbd>G</kbd> (Windows) or <kbd>⌥</kbd><kbd>⌘</kbd><kbd>G</kbd> (Mac).

To **ungroup** an existing model or folder, click the small arrow next to the button and select **Ungroup**. This action has a default shortcut of <kbd>Ctrl</kbd><kbd>U</kbd> (Windows) or <kbd>⌘</kbd><kbd>U</kbd> (Mac).

<img src="../assets/studio/general/Model-Tab-Group-Tools.png" width="706" alt="Group tools indicated in Model tab" />

## Lock tools

You can enable the **Lock Tool** by clicking the small arrow next to the **Lock** button and selecting **Lock&nbsp;Tool**. This action has a default shortcut of <kbd>Alt</kbd><kbd>L</kbd> (Windows) or <kbd>⌥</kbd><kbd>L</kbd> (Mac).

Once enabled, the tool operates as a "key" for both states&nbsp;&mdash; clicking on an unlocked object locks it, while clicking a locked object unlocks it.

To unlock all objects, click the small arrow next to the button and select **Unlock&nbsp;All**.

<img src="../assets/studio/general/Model-Tab-Lock-Tools.png" width="704" alt="Lock tools indicated in Model tab" />

## Anchor toggle

The **Anchor** toggle controls whether the part will be **immovable** by physics. When `Class.BasePart.Anchored|Anchored`, a part will never change position due to gravity, other parts collisions, overlapping other parts, or any other physics-related causes. This action has a default shortcut of <kbd>Alt</kbd><kbd>A</kbd> (Windows) or <kbd>⌥</kbd><kbd>A</kbd> (Mac).

<img src="../assets/studio/general/Model-Tab-Anchor.png" width="704" alt="Anchor toggle indicated in Model tab" />

## Solid modeling

The **Solid Modeling** section contains tools to create new geometry beyond the basic [parts](../parts/index.md) Roblox provides. For more information, see [Solid Modeling](../parts/solid-modeling.md).

<img src="../assets/studio/general/Model-Tab-Solid-Modeling.png" alt="Solid modeling tools indicated in Model tab" width="732" />

<table>
  <thead>
    <tr>
      <th>Tool</th>
	  <th>Shortcut</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Union**</td>
	  <td><kbd>Shift</kbd><kbd>Ctrl</kbd><kbd>G</kbd>&nbsp;(Windows)<br /><kbd>Shift</kbd><kbd>⌘</kbd><kbd>G</kbd> (Mac)</td>
      <td>Join two or more parts together to form a single solid union.</td>
    </tr>
	<tr>
      <td>**Intersect**</td>
	  <td><kbd>Shift</kbd><kbd>Ctrl</kbd><kbd>I</kbd>&nbsp;(Windows)<br /><kbd>Shift</kbd><kbd>⌘</kbd><kbd>I</kbd> (Mac)</td>
      <td>Intersect overlapping parts into a single solid intersection.</td>
    </tr>
    <tr>
      <td>**Negate**</td>
	  <td><kbd>Shift</kbd><kbd>Ctrl</kbd><kbd>N</kbd>&nbsp;(Windows)<br /><kbd>Shift</kbd><kbd>⌘</kbd><kbd>N</kbd> (Mac)</td>
      <td>Negate parts, useful for making holes and indentations.</td>
    </tr>
    <tr>
      <td>**Separate**</td>
	  <td><kbd>Shift</kbd><kbd>Ctrl</kbd><kbd>U</kbd>&nbsp;(Windows)<br /><kbd>Shift</kbd><kbd>⌘</kbd><kbd>U</kbd> (Mac)</td>
      <td>Separate the union or intersection back into its individual parts.</td>
    </tr>
  </tbody>
</table>

## Physical constraints

The **Constraints** section contains tools for creating physical `Class.Constraint|Constraints` between objects.

<img src="../assets/studio/general/Model-Tab-Constraints.png" width="754" />

Constraints are categorized into two groups:

- [Mechanical Constraints](../physics/mechanical-constraints.md) &mdash; Constraints in this group behave as mechanical connections, including hinges, springs, motors, and ropes.
- [Mover Constraints](../physics/mover-constraints.md) &mdash; Constraints in this group apply force or torque to move one or more assemblies

## Effects and spawns

The **Gameplay** section tools allow you to insert beautiful effects like [lights](../environment/index.md) and [particle emitters](../effects/particle-emitters.md), as well as quickly insert a `Class.SpawnLocation` into the 3D space.

<img src="../assets/studio/general/Model-Tab-Effects-Spawn.png" width="754" alt="Effects and Spawn tools indicated in Model tab" />

<table>
<thead>
  <tr>
    <th>Action</th>
    <th>Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>**Effects**</td>
    <td>Creates a new light or effect within the workspace or the selected object. The dropdown lets you select which type of effect to create.</td>
  </tr>
  <tr>
    <td>**Spawn**</td>
    <td>Adds a `Class.SpawnLocation` for players to appear at when they join the experience.</td>
  </tr>
</tbody>
</table>

## Advanced options

The **Advanced** section contains tools to insert advanced objects, services, and scripts, as well as configure [collision filtering](../workspace/collisions.md#collision-filtering).

<table>
<thead>
  <tr>
    <th>Action</th>
    <th>Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>**Insert Object**</td>
    <td>Opens the <b>Insert Object</b> popup for quick insertion of objects.</td>
  </tr>
  <tr>
    <td>**Model**</td>
    <td>Allows you to import a `Class.Model` from a local file.</td>
  </tr>
  <tr>
    <td>**Service**</td>
    <td>Allows you to insert services which are not listed in the Explorer by default.</td>
  </tr>
  <tr>
    <td>**Collision Groups**</td>
    <td>Opens a window which lets you create and edit collision groups for physical [collision filtering](../workspace/collisions.md#collision-filtering).</td>
  </tr>
  <tr>
    <td>**Run Script**</td>
    <td>Runs a `Class.Script` located in a file on your local machine.</td>
  </tr>
  <tr>
    <td>**Script**</td>
    <td>Inserts a `Class.Script` into the selected `Class.Instance`.</td>
  </tr>
  <tr>
    <td>**LocalScript**</td>
    <td>Inserts a `Class.LocalScript` into the selected `Class.Instance`.</td>
  </tr>
  <tr>
    <td>**ModuleScript**</td>
    <td>Inserts a `Class.ModuleScript` into the selected `Class.Instance`. You can implement his type of script to reuse code across other scripts.</td>
  </tr>
</tbody>
</table>
