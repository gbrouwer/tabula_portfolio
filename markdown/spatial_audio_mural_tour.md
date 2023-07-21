#h1 Spatial Audio Mural Tour

#h3 1 - Goal
#pg New York City, especially its borough of Brooklyn, has many amazing murals across many neighborhoods. Typically, people would design a mobile app that shows a map with locations of various murals to visit. However, I feel that using our smart devices like our iPhones as tiny laptops to be looked at and interacted with like they have keyboards does grave injustice to the affordance these devices offer. So, how can we utilize the devices more naturally while not getting distracted looking down at a screen and crossing a busy intersection without looking?

#im ../assets/spatial_audio_mural_tour/1.png 50 512 Figure 1 - A few murals in Brooklyn

#h3 2 - Innovation
#pg As a personal project, I decided that spatial audio is a more natural way to be alerted and find murals across the city. Using a pair of stereo headphones, the GPS capabilities of the smartphone, and a database of murals, your phone can determine the four closest murals to your location. Not only that, it can also compute the angle between your walking direction and the location of the murals. As such, we use some form of audio emanating from each mural, with its panning left to right, indicating what direction each mural is in. If a mural is to my northwest, it will ping audio panned to the left. Should the mural be behind me, it will fall silent. Although 3D audio exists that can create the illusion of something being in front or behind you, this is extremely expensive and not necessarily compatible with a regular smartphone. The distance of the mural relative to the user is indicated by volume, and the number of murals that can simultaneously 'call out' is also a setting the user can adjust. As for the audio ping, this can be a variety of sounds. Perhaps a piece of music (e.g., the mural of Biggie Smalls on Fulton Street), some narrative about the artwork's meaning, or maybe a simple ping would suffice. Although initially, the concept had the screen completely blank to minimize eyes on the device, but for demo purposes, the below version was created. 

#im ../assets/spatial_audio_mural_tour/2.png 50 384 Figure 2 - Mock version of the four closet murals, their distance and angle from the user and their walking direction

#h3 3 - Impact
#pg In addition to having people enjoy the many amazing murals New York City has to offer, this, for me, is an exercise in the affordance of our smartphones. Again, we still use them as little laptops, which defeats their value to me. 

#h3 4 - Alternatives
#pg Murals are one of many categories of places we can model using the same technology. We can switch it to Subway mode, where different subway lines 'call out' so you can easily find a stop suitable for transportation. Restaurants, grocery stores, landmarks, famous movie/tv sets, all of these place categories can use the same technology, provided there is an exhaustive list of these places as a database. 

#im ../assets/spatial_audio_mural_tour/3.png 50 384 Figure 3 - Murals are obviously not the only type of places of interest. The App can easily be set to other places, like nearby subway stops.

#h3 5 - Technologies Used
#br 
#it ../assets/logos/swift.png 0 96  
#it ../assets/logos/xcode.png 0 96 
#it ../assets/logos/ios.png 0 96
#it ../assets/logos/ios.png 0 96

