#Monday 24 March

##Team meeting — new teammate joined, unfamiliar with the project, thorough team meeting
Onboarded them on the codebase and project goals - delegated the commentary that was merged and assigned implementation
Nearly finished the merging of all branches into one universal branch
Confirmed race engineer running in mock mode
Verified Ollama running with granite4:3b
Ran test suite — all passing



#Tuesday 25 March

Started novice_wrapper.py
Beginner users were able to look at the simple configs inside the .py file and adjust them and see a direct reflection of their decisions in the way the car drove
Patched main.py to include commentary
Tested in mock mode — commentary fired correctly after 20s

Roadblock ran into as Commentary caused a bug in live TORCS and caused the car to spin out
Fix: Increased interval to 45s, load Ollama after TORCS connects

Wednesday 26 March

Continued the novice_wrapper.py

3-variable plain English config
Speed/corner/damage profiles
Live terminal dashboard
Full TORCS UDP connection

##Challenges faced:
The novice_wrapper couldnt work in tandem with the commentary, as it connected the car wouldn't be able to function and spun out



#Thursday 27 March

Completed the novice_wrapper:
Compromise was made to make the novice_wrapper functional whilst also maintaining the core aspect of the feature

It would be seperate from the AI commentary and racer engineer to keep the car's speed, steering, corner turn behaviour, etc, consistent with the novice's configuration options

Planned and started the livery_wrapper:
Takes car texture + university logo
Safe zone protects IBM branding
Pillow alpha compositing
--preview flag for before/after window
ImageMagick support for .rgb TORCS format



#Friday 28 March — Demo Day
.rgb files for the car in torcs didnt coincide with the actual vehicle on the race track, once the png file was implemented on a cars design 

CPU spikes from Ollama disrupted 50Hz driving loop
Car was spinning out when engineer loaded

Full test session in VM — all features passing
Wrote TESTING_PLAN.md with Gherkin UAT scenarios
Attempted live TORCS + engineer integration

Unable to make it to the client presentation due to the fact that the car was still compromised as the ai engineer and commentary connected