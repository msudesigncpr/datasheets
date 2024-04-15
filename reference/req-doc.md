
- Obj 1)	The system must identify target colonies.
	- Req 1.1)	The system must capture the locations of wells.
		- Spec 1.1.1)	The system must know the location of the center of each well to within 2 mm. 
		- Spec 1.1.2)	System must know the location of 96 wells on well plates that have been loaded by a technician.
	- Req 1.2)	The system must capture an image of an individual Petri dish. 
		- Spec 1.2.1)	Image resolution must be 0.25 mm per pixel or better. 
		- Spec 1.2.2)	System must capture an image of the entire petri dish at least 95% of the time.
		- Spec 1.2.3)	Estimated coordinates of target colonies that are sent to the motor control software must be accurate within 0.50 mm. 
	- Req 1.3)	The system must determine if a potential colony is valid for sampling.
		- Spec 1.3.1)	Target colonies must be valid colonies with a reliability of 95% or better, where a valid colony is defined as a colony that is not within a user-specified minimum distance of another colony.
		- Spec 1.3.2)	System must have a false positive rate for target colonies of 5% or less.

- ---

- Obj 2)	The system must transport a sample of each identified target colony to a unique well. 
	- Req 2.1)	The needle must be sterilized to prevent cross contamination.
		- Spec 2.1.1)	The needle tip must be inserted to a depth of at least 2 cm below the surface of the beads.
		- Spec 2.1.2)	The needle must not deform within 8 runs of 96 samples/run.
	- Req 2.2)	The needle must be moved into contact with an identified colony.
		- Spec 2.2.1)	The system must have a steady-state position error on the horizontal axes of less than ±0.5 mm relative to the center of the identified colony.
		- Spec 2.2.2)	The system must have a steady-state position error on the vertical axis of less than ±1.0 mm.
	- Req 2.3)	The needle with the colony sample must be moved to a well.
		- Spec 2.3.1)	The needle must be moved to the center of the well within 3 mm.
		- Spec 2.3.2)	The system cannot reuse a well 95% of the time.
	- Req 2.4)	This cycle must repeat until all target colonies have been sampled.
		- Spec 2.4.1)	All user-specified dwell times must be matched within a margin of 0.5s or better during each cycle.
		- Spec 2.4.2)	A full sampling cycle for a single colony must be completed in 30s + dwell times.

- ---

- Obj 3)	The system must accept user-specified parameters and record them alongside information associated with each sample.
	- Req 3.1)	The system’s code must allow for the user to start, pause, and stop sampling.
		- Spec 3.1.1)	The system must be able to start and pause within 2 seconds of the user’s command 95% of the time.
		- Spec 3.1.2)	The system must be able to stop within 1 second of the user’s command 95% of the time.
	- Req 3.2)	The system’s code must allow for the user to enter a label for each Petri dish on the baseplate.
		- Spec 3.2.1)	The system must allow for a unique label for each petri dish.
		- Spec 3.2.2)	The system must be able to store labels of up to 20 characters.
	- Req 3.3)	The system must record information about the samples collected. 
		- Spec 3.3.1)	The system must record how much total time it took for each sample cycle within 1s precision.
		- Spec 3.3.2)	The system must correctly record which Petri dish each sample originated from and which well each sample was deposited into 95% of the time.

---

Constraints :
•	Must use Festo motors and electronics selected by prior design group. 
•	Must use hot bead sterilizer selected by prior design group.
•	Must be operable with standard size Petri dishes and well plates.
•	Must use the existing frame without significant modifications.


