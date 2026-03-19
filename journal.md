# This is the journal of the (rather fast) design process, and eventual build process (less fast) of my custom toolhead, RFPToolhead.


## Journal Entry 1 3/19/2026
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
