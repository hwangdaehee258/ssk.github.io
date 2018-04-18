---
title: Hero(Player Character)
permalink: /docs/change_mesh_hero/
---

### Changing character's mesh

We are going to change character's mesh shown below.

![001 preview](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/001 preview.png "001 preview")

In the launch browser, click Marketplace button. and then type **Khaimera** in search box. you will see Khaimera asset. select **Paragon: Khaimera**.

![002 search for a new character(Khaimera)](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/002 search for a new character_Khaimera.png "002 search for a new character(Khaimera)")

Click **Add To Project** Button to download.

![003 add to project](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/003 add to project.png "003 add to project")

In the Content Browser, under **3DSideScrollerKit/Blueprints/Characters**, select **BaseHeroBP**.

![004 search for BaseHeroBP and select BaseHeroBP](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/004 search for BaseHeroBP and select BaseHeroBP.png "004 search for BaseHeroBP and select BaseHeroBP")

right-click on **BaseHeroBP**, and then click **Create Child Blueprint Class**

![005 right-click BaseHeroBP and Click Create Child Blueprint Class Button](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/005 right-click BaseHeroBP and Click Create Child Blueprint Class Button.png "005 right-click BaseHeroBP and Click Create Child Blueprint Class Button")

Name this blueprint **KhaimeraHeroBP**.

![006 change name and double click to open](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/006 change name and double click to open.png "006 change name and double click to open")

In the Content Browser, under ParagonKhaimera/Characters/Heroes/Khaimera/Meshes, double-click **Khaimera_Skeleton** to open.

![007 search for skeleton and double-click skeleton(khaimera)](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/007 search for skeleton and double-click skeleton_khaimera.png "007 search for skeleton and double-click skeleton(khaimera)")

Click **Options** Button. Click **Show Retargeting Options** Check Button.

![008 change option](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/008 change option.png "008 change option")

Click **Animation** Button shown below. and then select **Recursively Set Translation Retargeting Animation**.

![009 change option 2](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/009 change option 2.png "009 change option 2")

Click **Animation** Button show below. and then select **Animation Scaled**.

![010 change option 3](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/010 change option 3.png "010 change option 3")

Click **Retarget Manager** Button. and then Click Select Rig drop down button. select **Select Humanoid Rig**.

![011-1 select retargetmanager and change humanoid rig](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/011-1 select retargetmanager and change humanoid rig.png "011-1 select retargetmanager and change humanoid rig")

Click **Auto Mapping** Button.

![011-2 click auto mapping button](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/011-2 click auto mapping button.png "011-2 click auto mapping button")

Click **Save** Button.

![012 save options](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/012 save options.png "012 save options")

In the KhaimeraHeroBP, select Mesh. click Skeletal Mesh drop down button. and then select **Khaimera_WhiteTiger**.

![014 change mesh to Khaimera](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/014 change mesh to Khaimera.png "014 change mesh to Khaimera")

In the Content Browser, under 3DSideScrollerKit/BaseCharacters/Hero, right-click PaladinAnimBP to click **Duplicate Anim Blueprints and Retarget**.

![015 creating a new animation blueprint](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/015 creating a new animation blueprint.png "015 creating a new animation blueprint")

you will see **Select Skeleton** window shown below. select Khaimera_Skeleton and then Type **Paladin** in the Relpace box and **Khaimera** in the with box. click **Retarget** button.

![016 retargeting to khaimera](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/016 retargeting to khaimera.png "016 retargeting to khaimera")

Click **Save All** button.

![017 save all files created](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/017 save all files created.png "017 save all files created")

right-click on **3DSideScrollerKit** to create a new folder. Name a new folder **Khaimera**.

![018 creating a new folder](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/018 creating a new folder.png "018 creating a new folder")

select animation files and then move to **Khaimera** folder.

![019 move new files](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/019 move new files.png "019 move new files")

In the KhaimeraHeroBP blueprint, select **Mesh(Inherited)**, click **Anim Class** drop down button to select **KhaimeraAnimBP**.

![020 select new animation blueprint created](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/020 select new animation blueprint created.png "020 select new animation blueprint created")

In the Content Browser, under **3DSideScrollerKit/BaseCharacters/Hero/AnimMontage**, select all anim montage files and then right-click to **Duplicate Anim Assets and Retarget**.

![021 creating a animation montage](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/021 creating a animation montage.png "021 creating a animation montage")

select **Khaimera_Skeleton**, type paladin in Replace box and khaimera in with box and then click **Change...** button to select **/Game/3DSideScrollerKit/Khaimera** path. click **Retarget** button.

![022 retageting animation montage](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/022 retageting animation montage.png "022 retageting animation montage")

In the KhaimeraHeroBP blueprint. change Anim Montages show below.

![023 chainging animation montage in blueprints1](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/023 chainging animation montage in blueprints1.png "023 chainging animation montage in blueprints1")

![023 chainging animation montage in blueprints2](https://hwangdaehee258.github.io/ssk.github.io/img/changing mesh and animations/023 chainging animation montage in blueprints2.png "023 chainging animation montage in blueprints2")

![001 open animation blueprint and double-click idle_sword to open](https://hwangdaehee258.github.io/ssk.github.io/img/changing hero to new animations/001 open animation blueprint and double-click idle_sword to open.png "001 open animation blueprint and double-click idle_sword to open")

