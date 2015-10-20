# Electrodes
This page is all about electrodes!!
Interested about the other components of Stage 1?
* [[neurostimulator]]
* [[controller]]

## Overview

## Use Logging
Log anything that happens to an electrode, including test results, in the [Observation Log](https://pacific-basin-8674.herokuapp.com/admin/observation/?sort=4&desc=1)\! 
See this internal link [Observation Log](observation log) for more info.

## Troubleshooting
If you encounter impedance problems with an electrode, try the following tests to figure out why it may not be working.
For all tests, make sure the electrode is properly salinated (by either brining & water spray or soaking in saline).

### Nib to Nib
This is an ease test to quickly assess whether a pair of electrodes is working sufficiently.
1. Soak the electrode
2. Place one lead into the electrode’s lead slot
3. Place the other lead into another electrode’s lead slot
4. Touch all nibs of one electrode to all nibs of another. Some shear force will be needed to get a good connection.
5. Normal impedance is **<1500 ohms**
6. Record in [Halo Field Observations DB](https://pacific-basin-8674.herokuapp.com/admin/observation/?sort=4&desc=1) (Since the test requires two electrodes, be sure to include the SNs of each in the summary).
If this test fails, try the other tests to find out the specific problem.

![](https://photos-3.dropbox.com/t/2/AABOj4ItEPvf5yGDL6so0rvK58HmUS5VLx8Q-MiXZ5eZww/12/480526477/png/32x32/1/_/1/2/Screen%20Shot%202015-10-20%20at%2010.52.45%20AM.png/EMTqyPIDGAYgBygH/eIhp5ztkyclZdKA0w5hcTCafmw7X9dP4zDyeLYoQ8kg?size=800x600&size_mode=2)

### Lead to Nib Test
This test will assess the nib and connection between the nib and electrode backplate.
1. Soak the electrode
2. Place one lead into the lead slot on the electrode
3. Place the other lead on the end of a nib
4. Normal impedance is **<1000 ohms**
5. Test on multiple nibs to see if there is a difference between nibs
6. Record in [Halo Field Observations DB](https://pacific-basin-8674.herokuapp.com/admin/observation/?sort=4&desc=1)
If this test fails, there is a problem with the nib itself and/or the connection between the nib and electrode backplate. Try the next test to figure it out!

![](https://photos-6.dropbox.com/t/2/AAD4KasdR2AwCEsQFC7Fre3_AktZCUbHjU0A1MHQ7OWJvQ/12/480526477/png/32x32/1/_/1/2/Screen%20Shot%202015-10-20%20at%2010.52.25%20AM.png/EMTqyPIDGAYgBygH/1_qtr5j3ssO7ZM3eH5rEUZjZafG1l-s1yqf6vWp58FI?size=800x600&size_mode=2)

### Across Nib Test
This test will assess the nib itself.
1. Soak the electrode
2. Place each lead on opposite ends of a single nib which failed the Lead to Nib Test
3. Normal impedance is **<800 ohms**
4. Test on multiple nibs to see if there is a difference between nibs
If this test fails, the nib itself is definitely one of the problems.

![](https://photos-1.dropbox.com/t/2/AAC5ylvHrq7qbWCNZ2DiB0uHD8kusvzsypKrWwpgzNQvWA/12/480526477/png/32x32/1/_/1/2/Screen%20Shot%202015-10-20%20at%2010.51.58%20AM.png/EMTqyPIDGAYgBygH/EjkY49x8UJeeHBElEhlEA8OEQG2I5IIlvzGn5amgCx8?size=800x600&size_mode=2)

## Manufacturing