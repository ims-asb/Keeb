**Refined version**, cuz my actual journal sucks and is really messy. recommended to read this one!!!
**NOTE: I do not inflate my hours. I just am really slow. And this is my first ship, so i have a lot of stuff to learn.**

07/17/2026-07/24/2026
Decided to pick this up, made my parts list here (i have changed a bit of stuff since then)
<img width="1500" height="880" alt="Screenshot 2026-07-19 at 8 52 14 PM" src="https://github.com/user-attachments/assets/d801cca3-aa73-4f59-8101-7fdd556314d5" />
I also decided what specs I want.
I used KLE (https://www.keyboard-layout-editor.com/) to make a layout for my keyobard in JSON, then used KBPlacer on Kicad to actually place the stuff on the pcb for me
which saves a lot of time and is also more accurate cuz it doesnt have the natural problems of accuracy that we, mere humans, do
So what i did between this time, i learned kicad, how to add stuff, wire, etc
also learned about label connections 
instead of drawing a wire across the schematic
to connect some stuff
i can just slap a label
on both ends
and kicad counts them as labeled
<img width="1500" height="880" alt="Screenshot 2026-07-19 at 8 52 14 PM" src="https://github.com/user-attachments/assets/d801cca3-aa73-4f59-8101-7fdd556314d5" />

07/25/2026-08/01/2026
Only really did two days, cuz my dad grounded me for the rest
I added the MCP23017, basically to expand my pin count a bit
cuz the nano didnt have enough GPIO left for my matrix
so i added the mcp which talks over i2c and gives me a buncha pins without needing more from the nano
I also watched a few youtube videos on kicad, and i learned how to change units on some stuff
And i finagled with the MCP and nano, aka wiring sda/scl between them to do the above

08/02/2026-08/09/2026
This week, I worked on finishing up the pcb
And then i realized i forgot to add leds
So i did that
And there was a buncha problems
Like how it was insanity for freerouting to route
oh and
did i mention that i was using freerouting?
prob not 
but cuz like
after i wired all the switches n stuff together
for some reason
it just decided to flip me off and remove all the wiring
so
i decided to use freerouting
and, like kbp, it saves time and effort
I also decided on using kalih hot swap switches
and use 
And, my diode's pads glued to the switch's pad
which meant courtyard collisions
So
I fixed them
08/10/2026-8/17-2026
I realized that the LEDs arent actually on the front of the plate, but are on the back and have a hole to shine through
i also switched it to back copper
and i finally fixed every pcb warning and error (209)
i have now added silkscreen, which means there will be errors
but they're all cosmetic soooo
its fine
:)
*NORMAL JOURNAL*
so my idea for a keyboard for keeb is
a modified 96% ANSI keyboard with, for the twist,
an oled screen
a I2C knob
RGB underglow
and potentially 8K polling

im gonna use the Orpheus Pico as the MCU
and yeah
more updates coming later

ok. updates!! 07/17/2026
we gonna get a 0.91" I2C OLED
and yeah
about 23 GPIO pins used
<img width="1500" height="880" alt="Screenshot 2026-07-19 at 8 52 14 PM" src="https://github.com/user-attachments/assets/d801cca3-aa73-4f59-8101-7fdd556314d5" />
more stuff, too lazy to do tho
07/19/2026
uhhhh
no. we are not getting a orpheus pico
so we gonna get the nice!nano 
which supports eventually 8k polling which i want
but yeah
im working on the PCB design
specifically connecting them diodes and switches
and learning how kicad works in general
gn!
(all day, 12 hrs. kicad is hard lol)
<img width="634" height="598" alt="Screenshot 2026-07-19 at 8 47 33 PM" src="https://github.com/user-attachments/assets/63ae5344-140e-41c3-860b-28e940a5e94f" />

07/27/2026
by the way, i needed 2 pins extra for the actual keys. so i had to add a part (which i hate), the mcp23017. this gives me some more pins i could use.
but anyways, im done!
i did some work yesterday, but i was too tired and forgot to submit the log for yesterday, so yeah
3 hrs yesterday + 3 hrs today
08/04/2026
hello!
so i took a little break from keeb, heres whats going on!
1. i forgot to add leds. im doing that rn. 
2, im switching to hotswap switches
so i have to change the footprints
upd: i did the first, and tried the second. it didnt work
so im doing that tmr
2 hrs today
08/05/2026
hello
im doing the hotswap switches rn
i gave it a shot yesterday, but it completely sh*tted my brain
so im doing it today
1 hr
(i also 
08/06/2026
ok. i decided im gonna go with millmax hotswap switches
my brain was fried so i didnt get to add much else
also, this is taking quite a bit of time
so i kinda wanna just wrap this up
so yh
i might cut a few stuff
just getting really tired of doing kicad
really confusing
hundreds of errors and warnings
4 hrs :(
(i sadly dont have a photo for this. really tired)
08/09/2026
hello
so 
ehm
there was a lot of problems
i fixed them
example of that
the pads with the diodes n stuff
yeah
they were glued together
i almost crashed out 😭
this is kinda insane
uhm
yeah thats basically what happend 💀
there were some other led problems
and yeah, mill-max switches are too expensive
so i switched to kalih hotswap switches
theyre cheaper
4 hrs
https://cdn.phototourl.com/free/2026-08-14-67eb93e0-09e8-473c-a146-9330d93bb8ab.webp

08/11/2026
Hi.
YEah.
The leds didnt work.
I tried making them northup.
They don't work.
South, same thing.
Left is hella weird. 
So. 
wait uh nvm
its at back so it doesnt matter anyways XD
this is kinda stupid
3 hrs
https://cdn.phototourl.com/free/2026-08-14-bb5324b8-3c57-4740-8c53-ca2875367040.webp
what happened when i tried to put leds on the left 😭
08/12/2026
ok
uhh
i lost everything.
i tried to put the pcb and sch files in the git to give it to yall
but it for some reason overwrited my latest version with a really old one
so i had to restart
but yeah
i got back all my old progress
cuz the only different stuff is that 
1, the leds werent on the pcb
2, the nano, mcp, etc were placed wrong
3, leds were still named D instead of LED
so yeah
eveyrthing else was fine tho
1 hr
https://cdn.phototourl.com/free/2026-08-14-2dcdc610-ba33-4833-9f9d-150a059c6909.png
08/13/2026
so the board wasnt fully drc clean, had 209 violations when i hopped off yesterday
but 199 of them were cuz power to the leds were too close (under 0.5mm clearance)
but i did some research
and it seems like thats way too strict
cuz jlcpcb can support minimal of 0.2mm
so i set my board rule to 0.22mm for some wiggle room
and that basically cleared everything 
other than a few stragglers
which i did by hand
but i also had a short
where both nano battery pins were labeled differently
so i labeled them the same
second to last thing, there were 26 matrix gaps so i fixed those
and finally, i added more detail to this journal
cuz i was really lazy
but after 6 hrs of work
0 errors on the pcb!!!
im gonna add some silkscreen art tmr
then im gonna move to the case!
6 hrs
https://cdn.phototourl.com/free/2026-08-14-fb163dd6-1428-43de-a129-8ac2ebec5188.png
amazing rerouting work
08/14/2026
ok, so
i swapped to the kalh switches (CPG151101S11)
so it can hot-swap
and then i ran into a issue where the kalih switches are ever so slightly larger than the normal ones
so 
i had to kbp them again
so i fixed that
and then i had a mini heart attack
cuz when i was turning on freerouting to pick up some stragglers
i accidentally like
closed java instead of pressing the terminate button
so 
i freaked out for a bit
and then
i tried it again
and it came back!!
that scared the hell out of me
but anyways
i had like 209 drc errors
but then i checked jlcpcb's minimum board clearance
i finished the last stragglers (113!!! that freerouting didnt route)
and yeah
drc clean!
im currently working on the case
this is my kind of specialty
cuz i'm starting a 3d printing business
and i know how to 3d model
so yeah!
btw, for the case, i chose the top mount with padding, aka "poor man's gasket" mount. i also am adding kickstand legs to the case.
i also decided that it would be black with red accents (like my kitchen lol) and the pcb would be black, so the silkscreen would be white.
6 hrs
08/16/2026
ok
ehm
i took a day break
but 
i did some bit of progress
i moved the 4pin encoder so it has enough clearance between the screen
https://cdn.phototourl.com/free/2026-08-17-d89a887b-1f1f-422b-9688-a50732051218.png
yeah that was basically it 💀
i did start on the case though
i also decided to switch to gasket mount
cuz its still quite simple

1hr
08/17/2026
silkscreen!!!!
im also starting to work on the case
https://cdn.phototourl.com/free/2026-08-18-bad09f30-7c7e-4a81-ac93-e558f269b94c.png
08/18/2026
hi. im working on the silkscreen
again
and i worked on the case again
and thanks to @elslie for silkscreen art!
https://cdn.phototourl.com/free/2026-08-20-d2a7ba99-6f4e-4003-87d0-d18526cfb18e.png
very wow
absoultely amazing job
4 hrs
08/19/2026
had legal camp, so nothing
0 hrs
08/20/2026
casey casey! eggs and bakey!
finished my legal homework, so i have a bit of time
ok
