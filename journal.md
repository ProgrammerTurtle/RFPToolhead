# This is the journal of the (rather fast) design process, and eventual build process (less fast) of my custom toolhead, RFPToolhead.

## Total Time Spent: 18 Hours

## Journal Entry 1 3/18/2026
Time Spent: 5 Hours

Let's get things started. I am speedrunning this for the end of rework, so I better make it count. 
I started with the hotend. That's what this whole journal entry will be.

I spent about 20 minutes talking to various friends in the 3DP community and scanning prices before decidng on a supervolcano melt zone length. This is about 51.5mm, which is about 30mm less than my other hotend design and makes it much more usable for everyday printing. 

As per last time I:

<img width="387" height="452" alt="image" src="https://github.com/user-attachments/assets/e54a68b2-8ae1-40e6-a3d8-691c19d6373a" />

Started with a sketch of my nozzle and heater location and a rough shape. 

<img width="564" height="690" alt="image" src="https://github.com/user-attachments/assets/eead5592-7fcb-43ea-8f26-a3ccdec0fc7a" />

From there I extruded and added the meltzone tapping, as this will be using a supervolcano melt zone adapter and standard v6 nozzles. The little step at the top is because supervolcano heaters are only 47.5mm while the block needs to be 50mm, so this shaves off a little weight and reduces risk of shorting the heater. 

<img width="473" height="885" alt="image" src="https://github.com/user-attachments/assets/0d000b8a-bc1d-4ea8-8f24-3cb052681f16" />

From there I started playing with weight saving patterns! It only adds like $3 in machining but makes it look way cooler and saves a lot of weight. 

<img width="661" height="826" alt="image" src="https://github.com/user-attachments/assets/40dac5e4-0708-4f09-9769-47d3f2cb6d12" />

I then added all the holes. 4 holes in line with the heater, all tapped to M3, for two grub screws and two M3 stud thermistors. 
There are also 4 more M3 tapped holes that are 2mm deep. Two up top, two at bottom. This allows me to mount the hotend extremely rigidly to the SLM fan duct/toolhead unibody. 

<img width="535" height="1043" alt="image" src="https://github.com/user-attachments/assets/345c3644-3892-4ef1-80a8-78750adcf52e" />

<img width="679" height="977" alt="image" src="https://github.com/user-attachments/assets/4a7c9cbb-8883-4b8b-9907-9f3e26bf512e" />

After that, I added internals and the hotend was done! I know I kinda sped through this - that is not because it took a short amount of time. I went through 3 variations of cutaway patterns (basically I would make it look cool, send it to my machinist friend, and they would tell me if possible. rinse and repeat, I did a lot of filleting and chamfering - no fillets survived to the final product) and had to do a lot of research to find accurate sizing for components (apparently v6 nozzles can have two different thread lengths???). Fun fact! I designed that heatbreak manually based off a drawing I found online. Great skill to have btw. 

We get right about 51.5-53mm of meltzone, which should be plenty for my uses! 

Also, about the weight savings I mentioned earlier...
The block weighs 13 grams. That's it. It's WILD. Comparable supervolcano block is like 100 grams.

<img width="380" height="776" alt="image" src="https://github.com/user-attachments/assets/bede6123-b5a7-405e-bd5a-1482873e088b" />

Sneak peak at what is coming! I am actually really excited for this project. 

## Journal Entry 2 3/19/2026
Time Spent: 8 hours

<img width="762" height="973" alt="image" src="https://github.com/user-attachments/assets/cba14a1a-c822-4574-b34b-2bfcdf16a66f" />

Yes, that's right. 8 hours. My excitement I mentioned earlier? That was a little bit of a mistake. 
Duct design hurts a little sometimes.

That photo up above is a pretty big leap from where we left off ! Let's take a few steps back. 

<img width="736" height="1025" alt="image" src="https://github.com/user-attachments/assets/ab4f9a13-ab24-4193-9e6b-f1b7b5d409dd" />

I started off with the outlet of the ducts. This was some simple sketching to determine sizing and angle from the ground plane, and then an extrusion to represent the path I need the air to be taking at the end of the duct.
The outlet sizing is relatively simple. Take your inlet cross sectional area and maintain that area throughout the entirety of the duct (or you can shrink to like 80% or smth but I like 1:1). In this case, with a 19mm ID cpap tube I have aout 200mm^2 of cross sectional area. So, I sized my outlet to 20mm x 10mm, to get 200mm^2. 
Wait, what?
But aren't there two outlets?
Yeah. I messed this up and didn't realize until after about 6 hours of duct design. I will cover how I fixed it when we get to that point, but just know that it should be 100mm^2 per side (I did about 5mm x 20mm). 

Anywho, from there I copied the outlet cross section a few times and used them to structure my duct. By placing cross sections at points I want to control, I can then loft between them and have my duct. Some people will just do one cross section sketch and then sweep along a 3D-sketched line path. I don't like this approach as it is very difficult for me to visualize my duct in that manner. 

<img width="699" height="366" alt="image" src="https://github.com/user-attachments/assets/38262587-e52d-461b-8024-4dfe86b4d780" />

<img width="497" height="996" alt="image" src="https://github.com/user-attachments/assets/8e51dc2c-8dc6-4ea6-9acc-51717c56d1dd" />

<img width="575" height="877" alt="image" src="https://github.com/user-attachments/assets/9f35e257-e937-40c0-8053-f509dba10783" />

I stacked them up from bottom to top, like the progression of those photos, maintaining my cross sectional area the whole way up. Important note: I did not get this right the first time. Or the fifth time. Or the 20th time. I basically just had to keep making small adjustments and redoing the lofts to see how my duct shape changed. 

<img width="558" height="896" alt="image" src="https://github.com/user-attachments/assets/ebb0ecfd-759d-4744-bb3c-afa057ab233f" />

<img width="517" height="1078" alt="image" src="https://github.com/user-attachments/assets/83a7e7de-de60-459e-8c59-68e1331d1719" />

<img width="754" height="1012" alt="image" src="https://github.com/user-attachments/assets/05648c9d-6fbb-42a1-ac18-8c2df65cdcd0" />

<img width="654" height="1051" alt="image" src="https://github.com/user-attachments/assets/3aef44f8-f438-48c5-9c43-bedc19a1de2c" />

You can see some of that process here as the shape changes over time, with the changes getting less and less drastic with each revision. Eventually I was making millimeter adjustments. 

You may notice that the duct randomly got thin during that photo progression ! That was at about hour 6 as I mentioned earlier, where I realized my mistake with the cross section and had to fix it.

<img width="830" height="938" alt="image" src="https://github.com/user-attachments/assets/aad665c4-0398-4a72-9d2c-a1fa1c42b806" />

This is unfortunately what that process looked like, and it managed to take an hour ish. I had to go through each cross section sketch and cut it in half. For the sketches that were not parallel to the ground plane I had to construct a new plane to sketch off of because fusion is silly. I also made some adjustments to overal shape here yet again as the thinner duct let me pull the sides in even closer to the hotend/extruder, making the toolhead less wide. 

<img width="667" height="962" alt="image" src="https://github.com/user-attachments/assets/0752930b-8527-446c-9cb6-297d96ab09a9" />

A quick mirror and we have the ducts ! From here I started working on the actual toolhead structure. 

<img width="1121" height="893" alt="image" src="https://github.com/user-attachments/assets/fa40edbc-a8d1-4084-b27d-e9364d1c0310" />

First I pretty simply joined the outlets together. This allows for easier hotend bracing, convection shielding for the hotend, and greater structural rigidity. 
There is a 10mm hole so I can fit a nozzle wrench around the nozzle. This makes toolhead assembly possible and nozzle changes way less inconvenient. I am looking into a thin bent sheet metal piece (or rather two) that I could slot in to cover the hole. 

<img width="696" height="1115" alt="image" src="https://github.com/user-attachments/assets/895d6ff5-21e8-436f-88bd-e39fe6a45f83" />

Next is the extruder mount and heatbreak interface. This is effectively what makes the toolhead the hotend heatsink, allowing for heatbreak cooling both via surface radiation of heat and cpap air. 

I did this pretty simply by making a sketch at the base of the extruder that intersected the ducts, allowing me to bridge the space between the two. 

<img width="1317" height="544" alt="image" src="https://github.com/user-attachments/assets/98558d57-b597-4649-ae56-51162bbe665e" />

And then it gets fillets and chamfers to be pretty ! 

<img width="1015" height="608" alt="image" src="https://github.com/user-attachments/assets/a639c80e-cca6-4fad-aeba-24f56e3c3700" />

Last but certainly not least I did the hotblock bracing. 

<img width="940" height="450" alt="image" src="https://github.com/user-attachments/assets/b4b8b785-3c3a-4b0e-a0cc-886a676527e1" />

These are pretty simple "struts" that bolt to the block with M2 screws. You can see that the section that actually contacts the block is cut away to minimize contact, allowing for thermal isolation (hopefully). 

<img width="656" height="621" alt="image" src="https://github.com/user-attachments/assets/e780c681-1e8e-4458-aad2-3d7ac9577949" />

And that is actually it for this entry ! I was up until about 6:30 AM doing this stuff. Duct design is super tedious but honestly I found it really calming past about 3am. It was really nice actually. 

Next is probe mounting and belt clamps, then this bad boy is done ! I am excited. 

## Journal Entry 3
Time Spent: 5 hours 

This is the last CAD journal entry ! The next one will be all the logistics stuff for submitting. 
Basically, I need to mount a BTT Eddy Duo, and belt attachment points. 

<img width="1254" height="776" alt="image" src="https://github.com/user-attachments/assets/bf8e1e2d-6987-4fc1-b10a-1d1a18a8adde" />

I added a flat section to the rear for the probe to mount to. This took 2 hours as I had to do a lot of digging to find the required info for where the probe should be mounted. I also had a lot of issues with filleting things because fusion is fusion.

<img width="874" height="736" alt="image" src="https://github.com/user-attachments/assets/cb43c172-c6c9-47a2-a5f2-b3430d580183" />

It was a pretty simple sketch though, just projected the probe and the ducts then sketched a flat section to bridge the ducts. 

<img width="996" height="505" alt="image" src="https://github.com/user-attachments/assets/2a77988f-aa41-49f4-88e5-fef0e29dc70e" />

Then comes belt mounting ! I figured out the mounting location by copying it from my old toolhead, which was a spinoff of kevender/lh stinger toolhead. 

<img width="1336" height="1171" alt="image" src="https://github.com/user-attachments/assets/e63aa493-229a-4189-bcbe-8707fd4811ab" />

You can kinda see the similarities in belt mounting. The belts will be clamped with two m3 screws by a little lasercut steel piece from JLC. They will cost like 2 dollars and I will just be paying for them myself because getting a quote from JLC sheet metal is really annoying. 

I had a LOT of issues with this. I had to spend 2 hours messing with the model to get the geometry to stop crying. 

<img width="1164" height="1058" alt="image" src="https://github.com/user-attachments/assets/27254a7a-9df5-4636-b514-67a7601089f1" />

Basically this interior was all messed up and it wouldn't let me fix it. I ended up having to cut the model up to fix it. 

<img width="784" height="1074" alt="image" src="https://github.com/user-attachments/assets/8e253960-8a39-4b48-88cd-b6d606e0f3b2" />

You can see that here. Anywho, it got done after a lot of pain.
Oh! I forgot. 

<img width="784" height="1074" alt="image" src="https://github.com/user-attachments/assets/e6afe523-e81f-4496-8b25-18d944c4c97b" />

The remaining hour was spent on this little perch thing for the extruder motor. This is to hopefully increase rigidity on the top of the duct and potentially help cool the extruder motor a little since they get quite hot at high current. 

<img width="951" height="829" alt="image" src="https://github.com/user-attachments/assets/f10f2d95-39b7-4bbd-8699-640e96d2925c" />

I think it turned out rather nice but it did take quite a lot of effort to get the geometry to match what I wanted. 

<img width="862" height="705" alt="image" src="https://github.com/user-attachments/assets/ae1333e8-5684-4081-87eb-7c433561a524" />

You can see how it lines up with the ducts to not have anything sticking out any side but the front, and evem that bit is minimized. That was really annoying. 

<img width="1095" height="446" alt="image" src="https://github.com/user-attachments/assets/0664a515-8a98-4f8b-9bf6-aa2ee6defdc9" />

Anywho, I also did some renders ! Because... the toolhead is done ! 

<img width="2000" height="2000" alt="rfptoolhead front" src="https://github.com/user-attachments/assets/a826eb34-a9be-4a19-96ad-de384e2b67ac" />

<img width="2000" height="2000" alt="rfptoolhead side" src="https://github.com/user-attachments/assets/473669cc-0f2d-427a-8826-6ef70c2e502a" />

<img width="1151" height="2087" alt="rfptoolhead main" src="https://github.com/user-attachments/assets/081512ba-942c-46a8-8849-9d11049a5225" />

All that is left is logistics and submitting. 
