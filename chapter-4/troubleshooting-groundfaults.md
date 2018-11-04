# How to Troubleshoot Ground Faults and Shorts

### Overview

Once the programmer has determined which loop has the fault. Figure out the start and end of the loop, whether Class A or Class B. The ides behind searching for the fault is through dividing the loop in half each time; then determine which side has the fault present.

1. Isolate the loop from the Fire Alarm Control Panel; both feed and return for Class A. 
2. Determine if the fault is on the positive or the negative wire of the loop.
3. Locate and disconnect the middle device of the loop. This isolates one 'side' of the loop from the other.
4. Find what 'side' the fault is still present on. Then determine which direction, device, of the loop, the fault wire lead.
5. Then repeat Step 3 for that half of the loop. Continuing until the fault is located and fixed; or has disappeared after disconnecting and reconnecting the devices. 

### Fault Reading

**Continuity Method**

To test for a ground fault or short the easiest way is with the continuity function of a digital multimeter(DMM). On most meters when the leads have an impedance of less than around $${30}\Omega$$ the meter will yield a positive continuity reading; usually has a tone associated with a visual read out of the $$\Omega$$ value likely $${0}$$.

Make sure that the wires at the the start and end of the loop are isolated from the panel and not contacting any bonded metal parts (ie. the box they are in). Then at the middle device place one DMM lead on the bonded box or other bonded metal part, with the other DMM lead on the wire that is to be tested for the ground fault / short.

**Voltage Split Method**

The fire alarm panel will output roughly $${13}V$$ per wire of the loop. Meaning that from either the Red of Black wire to Ground would read $${13}V$$; with around $${25}V$$ between them. Sometimes the continuity setting is not sensitive enough to pick up the fault that the panel is reading; meaning there is some voltage bleeding off, but the resistance is still high enough to not have it show a full fault, either dead short or dead ground. 

The high resistance ground fault or short can still be detected with the voltage split method since any voltage higher than roughly 20V on one side will read as a fault to the panel; therefore not passing verification. The wire/size with the lower voltage reading is the one which has the high resistance fault present. Follow this just like the continuity above.


### Self Clearing Faults

During the process of trying to locate the fault, sometimes it will disappear (clear) without actually finding or fixing the problem. This can be caused by a few different reasons. 

1. When the device was removed from the box, the wires become stretched out of the box and therefore are no longer in contact with the metal box. As fire alarm is run with wire sizes normally 18-14ga, the small amount of insulation can become damaged while *pulling* wire; usually on the sharp edges of the boxes. This small cut can go undetected, and only becomes an issue when the device is mounted to the box and the wire is placed inside.
2. There can be some metal protrusion in the box the contacts the terminal screws of the device and either grounds or shorts them out. I have seen this happen do to the foil shield on the wire.


### Typical Fix

Normally the faults I have found have been a small cut in the insulation of the wire; which contacts the box when the device is mounted and wire placed inside. Typically I find the fault with it self clearing. In which case I determine where I last saw read the fault; inspect the device I just recently removed and use electrical tape to tape up the wire; as 33+ rated electrical tape has a [voltage rating of](https://multimedia.3m.com/mws/media/104792O/scotch-super-33-vinyl-electrical-tape-pdf-27-3kb.pdf) $${600}V$$.


### In Depth Problems

Occasionally the problem is worse then a wire in a box with a minor cut. I have seen where the wire has been striped during the manufacturing process with armored cable(BX), fire alarm cable. At that point a new cable will have to be run, which will take real time decisions to determine the best course of action. Hopefully the system was run with conduit and not BX.

