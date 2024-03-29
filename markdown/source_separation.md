#h1 Source Separation

#h3 1 - Problem Statement and Goal
#pg Intensive Care Units (ICUs) and Emergency Rooms (ERs) are extremely noisy and chaotic places in hospitals. They are filled with medical equipment that all produce various sounds. Some of these sounds are essential indicators, for example heart rate monitors. Other sounds are the inevitable result of care given and the communication between staff and patients. Within all of this, clinical staff will need to be able to hear specific alarms from a distance, as they cannot have eyes on every patient. However, a lot of the sounds are not relevant to anyone clinician. Patients are divided across clinicians, and each clinician must pay attention only to a subset of sounds. Similarly, not, if not all conversations at any time are relevant for anyone clinician. Family members converse in and outside rooms, in hallways, and clinicians at their stations. Finally, from the patient's point of view, most sounds are irrelevant, even those produced by the equipment they are attached to. They only really need to comprehend and understand things that are said to them, not necessarily to anyone else. Finally, perhaps they would prefer focusing on the sound from a TV for distraction, which is hard given the sounds that fill their rooms already. 

#h3 2 - Innovation
#pg In all the above examples, the real solution seems obvious: both patient and clinician should have some ability to tune in to specific sounds or voices while others are muted. Therefore, I experimented with a known technique called source separation that theoretically will allow for this, but as applied to a hospital setting, through means of simulation.

#h3 3 - ICA source separation 
#pg Independent Component Analysis is an algorithm that uses the statistical structure of a signal to divide it into separate sources. In other words, it is a mathematical technique to unmix several sounds into the different sources it is comprised of. I implemented this technique in a Unity-based simulation to demonstrate its usefulness. 

#im ../assets/source_separation/3.png 50 256 Figure 1 - To do source separation, we need multiple recording sites. By rotating our head from left to right, we obtain slightly different audio signals arriving at the patients left and right ear. Humans actually use the left and right ear for source separation, taking into account first and foremost the different in position, but also the complex audio shadow that the head itself casts on a sound coming from one side (e.g. left) on the right ear. 

#h3 4 - Simulation Design
#pg Using Unity and 3D LEGO pieces, I designed a hospital room containing various pieces of sound-producing equipment and is connected to a hallway producing background noise. 

#im ../assets/source_separation/1.png 50 256 Figure 2 - Schematic of the simulated hospital room. The patient is flanked on either side by two sound producing devices, and hallways sounds enter the room through the open door. 

#h3 4 - Simulation
#pg In the simulation, we take on the perspective of a patient being addressed by a clinician, with plenty of ambient noise and sound emanating from all directions. In the first video embedded below, you can see and hear how many different sounds reach the patient from all sides and that it is hard to understand the doctor, even when facing in their direction. However, the same conversation becomes much more intelligible after we apply source separation. 

#im ../assets/source_separation/2.png 50 292 Figure 3 - Different view points of the patient (A,B,C,D, and F) and the perspective of the speaking clinican (E). 

#h3 5 - Impact
#pg If a source separation algorithm can be implemented into an earpiece and operate with sufficient accuracy and in real-time, much in the same way our headphones have noise cancellation abilities, both patient and clinician can choose what sound(s) or voice(s) they want to be able to hear, and which ones should be muted as much as possible. In addition, by embedding context-aware artificial intelligence, such a system might itself switch 'channels' to alert a clinician of a sound or voice relevant to them that they otherwise might have missed. Finally, it can serve as a way to protect a patient's privacy by blocking a channel that contains a conversation between a patient and clinician or two clinicians discussing a patient for anyone who should not hear it. 

#h3 6 - Technologies Used
#br 
#it ../assets/logos/csharp.png 0 96 
#it ../assets/logos/unity.png 0 96 
#it ../assets/logos/python.png 0 96  
#it ../assets/logos/lego.png 0 96 
#it ../assets/logos/scikitlearn.png 0 96 
#it ../assets/logos/scikitlearn.png 0 96 

#br 
#h3 7 - Demo Videos



