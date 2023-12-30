I'm using my own no-cut mini DIN mount that requires the removal of the original S Video and RCA AV outputs. The mini DIN mounts in place of the S Video out, and the 240P switch mounts in place of the composite video out. If you don't mind cutting the case, you can just mount the mini DIN to the RF module location on the main board, and drill a hole through. This model had a provision for the module on the pcb itself, but it was never populated, nor was the case drilled for it.

As for the actual install, it's very straightforward, but requiers fairly advanced soldering skills for the flex cable.
* Solder the flex to the GPU. This is very fine pitch soldering, and is not beginner friendly at all.
* With the flex soldered in place, triple check that there are no bridges. If you don't have a microscope you can take well lit pictures and zoom in. Do not skip this step.
* Insert the flex into the RGB board, and secure on top of the GPU. These new ones don't have the double sided tape on the bottom, so I held mine down with some kapton tape for now.
* Run the RGB and sync wires to your AV connector of choice.
* You'll need to route ground to your AV connector.
* If you need a 5 volt line, you can gently scrape off the soldermask on the VCC pad right below the RF module spot on the board.
* Route left and right audio from the RCA connectors to you new AV connector.
* Might as well pull the composite signal as well, what's one more wire.
* If installing a 240P switch, you should, this part isn't documented anywhere for this console. You need to remove the 0 ohm resistor R170.
* With R170 removed, run a wire from the right pad of R170 or the already unpopulated R171 to the Hz0 pad on the 3DORGB board.
* Run a wire from the Hz1 pad on the 3DORGB board to the common pin on an SPDT switch.
* Leave one pin of the switch floating, not connected to anything. This is your 240P position.
* The other pin of the switch needs to be run to ground. This is your 480i position.

If you're using my no-cut miniDIN and switch mount, there are a few notes.
* Remove the RCA/S Video connector. It locks in place under the S Video connector, and it's difficult to remove here. I suggest melting the solder and trying to squeeze these locking tabs in a bit. Otherwise it is fairly easy to damage these pads as can be seen from my pictures. If these pads do get damaged, it's not a big deal. Take your time here.
* Clean up any residual solder and flux at this point.
* We are mounting the miniDIN upside down right over the S Video connection, so we need to put some kapton tape down to isolate everything.
* Assemble all the pieces without soldering anything to make sure everything is lining up correctly.
* With the rf and rca boards and miniDIN laying on the main board in their locations, tack solder in both boards.
* Double check the alignment of everything here. Make sure the miniDIN is lined up with the S Video hole in the case, very important.
* With the alignment correct, fully solder in the rf and rca boards.
* Solder on short wires to the luma and chorminance pads on the rca board, and route down the hole.
* Solder these to their respective pads under the board.
* Sandwich 2 switch spacers between the switch and the miniDIN board, double check that it's nice and perpendicular, and solder in place.
* Center the smd mount female headers on the rf and rca boards, and tack solder on. Double check alignment, and fully solder in.
* Place the male headers in the female headers, and put the miniDIN board in place.
* Clip the pins for the headers and miniDIN close to the board and solder in. Do not clip the 3 big shield pins.
* Place the shield board over the miniDIN board, clip the 3 shield pins, and solder in place.
* At this point you can fully test everything after the 3DORGB is fully installed.
* If everything is working as expected, you can solder in the miniDIN connector to the rf and rca boards for extra security. You don't need to do this, but this connector could loosen over time being held in only by the 2 8 pin headers. However, if don't don't solder the sides of the miniDIN connector, you can actually swap out this part with the 8 or 9 pin version.
