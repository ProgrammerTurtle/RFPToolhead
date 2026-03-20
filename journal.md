# This is the journal of the (rather fast) design process, and eventual build process (less fast) of my custom toolhead, RFPToolhead.


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

Journal Entry 2 3/19/2026
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
